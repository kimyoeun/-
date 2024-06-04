#include <stdio.h>
int main()
{
    int i,food;
    float sum=0;
    char a[7]={잠자기,식사하기,TV보기,이야기하기,공부하기,서 있기,빨리 걷기};
    float b[6]={0.9,1.6,1.1,1.6,1.9,2.1,4.2};
    int c[6];
    printf(“다음 활동을 몇시간 하였는지 답하시오”);
    for (i=0;i<=6;i++)
    {
        printf(“%s”,a[i]);
        scanf(“%d”,&c[i]);
        sum=sum+b[i]*c[i];
    }
    printf(“당신의 하루 섭취량은 %.f kcal입니다\n.“,sum);
    printf(“오늘 당신이 하루동안섭취한 음식은 총 몇 kcal입니까?:”);
    scanf(“%d”,&food);
    
    if(sum>food)
        printf(“지금과 같은 생활을 지속할 경우, 체중이 감소할 가능성이 높습니다.저체중을조심하세요.“);
    else if(sum<food)
        printf(“지금과 같은 생활을 지속할 경우, 체중이 증가할 가능성이 높습니다.비만을조심하세요.”);
    else
        printf(“정말 완벽한 생활을 하고 계시군요!);
    return 0;
}
