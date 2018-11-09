
// DOC -------------------------------------
//
//  Compile:     gcc main.c -lncurses
//
//
//
//
//
//-----------------------------------------
#include <stdio.h>
#include <stdlib.h>
#include <ncurses.h>

//--------------------------------------------------------------------------------------------------------------- VARIABLES
char last[10];
WINDOW * ma_fenetre;
//--------------------------------------------------------------------------------------------------------------- FUNCTIONS
int capture()
        {char nom[12]; system("clear"); printf("Quel est votre code ? "); fgets(nom,10,stdin);printf("Ah ! Tres bien ! Execution de: %s !",nom); memcpy(last, nom, 10); return 0; }
//---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
void welcome()
        {system("clear");printf("###################################################################\n");printf("System good!\n");return;}
        char pass[]="quit\n";
//-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
void _OpenCurse()
        {initscr(); int i=has_colors();int e=start_color();init_pair(1,COLOR_WHITE,COLOR_RED);attrset(COLOR_PAIR(1));wattron(ma_fenetre,COLOR_PAIR(1));move(5,15);printw("Hello World                                                                            !!!");refresh();getch();endwin();}
//----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
void Type(const char * p)
        {if (NULL ==p) return;while(*p){printf("%c",*p++);sleep(10);}}
//----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
void _CloseCurse()
        {delwin(ma_fenetre); endwin(); }
//---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
void Reader(const char *f)
        {FILE *fd;char *line[100];
        if (NULL==(fd = fopen (f,"r"))){fprintf(stderr,"IMPOSSIBLE TO OPEN.\n");exit(EXIT_FAILURE);}
        while (fgets(line,100,fd)){printf("%s",line);}
        if(!feof(fd)){fprintf(stderr,"TROUBLE TO READ\n");
        exit(EXIT_FAILURE);}
        fclose (fd);printf("\n");}
//-------------------------------------------------------------------------------------------------------------- MAIN
int main(int argc, char *argv[])
{

    welcome();
   // do{
   // capture();
   //     }
   // while(strcmp(last,ex)!=0);
    printf("...suite...");
    _OpenCurse();
    int c = getch();
    _CloseCurse();
    Reader("toto");
        return 0;
}
//--------------------------------------------------------------------------------------------------------------
