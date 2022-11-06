<template>
    <f7-page name="checkin">
        <f7-navbar title="Chấm công" back-link></f7-navbar>

        <f7-card shadow  outline>
            <f7-card-header>Thông tin chấm công</f7-card-header>
            <f7-card-content>
                <p>Giờ vào 7 giờ sáng: hoàn thành</p>
                <p>Giờ ra 05 giờ chiều: hoàn thành</p>
                <p>Tăng ca 2 giờ: chưa hoàn thành</p>
                <p>Tăng ca 4 giờ: không có</p>
            </f7-card-content>
        </f7-card>

        <f7-block>
            <p>Bước 1: mở ứng dụng google auth</p>
            <p>Bước 2: chọn mã của cty (bluecat)</p>
            <p>Bước 3: copy dãy 6 mã số (hoặc ghi nhớ)</p>
            <p>Bước 4: nhập hoặc dán vào ô mã số phía dưới</p>
            <p>Bước 5: bấm "CHẤM CÔNG" phía dưới</p>
        </f7-block>


        <f7-block>
            <f7-button class="width-150 m-auto" fill >Chấm công</f7-button>
        </f7-block>
    </f7-page>
</template>