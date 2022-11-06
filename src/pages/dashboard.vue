<template>
    <f7-page dark>
        <f7-navbar title="Dashboard"></f7-navbar>

        <f7-card no-shadow outline padding class="flex">
            <f7-card-header>
                <img src="https://cdn.framework7.io/placeholder/people-68x68-1.jpg" width="100" alt=""/>
            </f7-card-header>
            <f7-card-content>
                <p >Nguyễn Minh Trọng</p>
                <p>Bộ phận: Developer</p>
                <p>Hôm nay: 10/07/2022</p>
            </f7-card-content>
        </f7-card>

        <f7-block padding outline strong>
            <f7-card-content>
                <p>Chấm công: <span color="red">chưa thực hiện</span></p>
                <p>Ngày phép còn lại: 12</p>
                <p>Bạn có 10 thông báo</p>
            </f7-card-content>
        </f7-block>

        <f7-block>
            <f7-row>
                <f7-col class="text-center">
                    <f7-card outline>
                        <f7-link href="/request/" color="white" class="m-auto block p-10 ">
                            <f7-icon f7="house"></f7-icon>
                            <p>Nghỉ phép</p>
                        </f7-link>
                    </f7-card>
                </f7-col>

                <f7-col class="text-center">
                    <f7-card outline>
                        <f7-link href="/checkin/" color="white" class="m-auto block p-10 ">
                            <f7-icon f7="checkmark_2"></f7-icon>
                            <p>Chấm công</p>
                        </f7-link>
                    </f7-card>
                </f7-col>

                         
            </f7-row>

            <f7-row>
                <f7-col class="text-center">
                    <f7-card outline>
                        <f7-link href="/request/" color="white" class="m-auto block p-10 ">
                            <f7-icon f7="table_fill"></f7-icon>
                            <p>Công việc</p>
                        </f7-link>
                    </f7-card>
                </f7-col>       
                <f7-col class="text-center">
                    <f7-card outline>
                        <f7-link href="/request/" color="white" class="m-auto block p-10 ">
                            <f7-icon f7="bell_fill"></f7-icon>
                            <p>Thông báo</p>
                        </f7-link>
                    </f7-card>
                </f7-col>

                             
            </f7-row>
            <f7-row>
                <f7-col class="text-center">
                    <f7-card outline>
                        <f7-link href="/request/" color="white" class="m-auto block p-10 ">
                            <f7-icon f7="money_dollar_circle_fill"></f7-icon>
                            <p>Phiếu lương</p>
                        </f7-link>
                    </f7-card>
                </f7-col>

                <f7-col class="text-center">
                    <f7-card outline>
                        <f7-link href="/request/" color="white" class="m-auto block p-10 ">
                            <f7-icon f7="square_arrow_right"></f7-icon>
                            <p>Thoát</p>
                        </f7-link>
                    </f7-card>
                </f7-col>   
            </f7-row>

            
            
        </f7-block>

    </f7-page>
</template>