# BtnToEditListenerUtils
封装当EditText输入都不为空时，按钮才可以点击工具类

## 使用如此

       BtnToEditListenerUtils.getInstance()
                .setBtn(btnRegister)
                .addEditView(editPhone)
                .addEditView(editPwd)
                .addEditView(editPwd1)
                .addEditView(editPwd2)
                .addEditView(editVerify)
                .build();

        btnRegister.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Toast.makeText(getApplicationContext(), "Register", Toast.LENGTH_SHORT).show();
            }
        });
