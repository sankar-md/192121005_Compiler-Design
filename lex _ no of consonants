%{
int vow=0;
int con=0;
%}
%%
[aeiouAEIOU1234567890!@#$%^&*()_+}{:"<>?|`=\;'/.,] {vow++;}
[a-zA-Z] {printf("%s\n",yytext);con++;}
%%
int yywrap(){}
int main(int argc,char*argv[])
{
	yyin=fopen(argv[1],"r");
	yylex();
	printf("no of consosnants is :%d\n",con);
	fclose(yyin);
}
