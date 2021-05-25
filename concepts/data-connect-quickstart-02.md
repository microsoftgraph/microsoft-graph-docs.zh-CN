<!-- markdownlint-disable MD002 MD041 -->

在首次使用 Microsoft Graph Data 连接 之前，需要配置 Microsoft 365 租户。 这涉及打开服务并配置具有批准数据提取请求的权限的安全组。

## <a name="grant-azure-ad-users-the-global-administrator-role"></a>向 Azure AD 用户授予全局管理员角色

在此步骤中，将确保租户中的两Microsoft 365已启用 **全局管理员** 角色。

- [全局管理员内置角色](/azure/active-directory/roles/permissions-reference#global-administrator)。
- [提升访问权限以获得全局管理员角色](/azure/role-based-access-control/elevate-access-global-admin)。

## <a name="configure-microsoft-graph-data-connect-consent-request-approver-group"></a>配置 Microsoft Graph数据连接同意请求审批者组

在此步骤中，你将设置你的 Microsoft 365 租户，以允许使用 Microsoft Graph Data 连接。

1. 打开浏览器，然后转到你的Microsoft 365[门户。](https://admin.microsoft.com/)

1. 在边栏导航上，选择"**活动组"。**
  
    ![显示管理中心的活动Microsoft 365屏幕截图。](images/data-connect-m365-act-grp.png)

1. 选择" **添加组"** 按钮。

1. 使用以下方法创建新的启用邮件的安全组，然后选择"**添加"** 按钮。
   - **类型**：启用邮件的安全性

    ![Screenshot showing a user selecting the mail-enabled security for a new group in the Microsoft 365 admin center.](images/data-connect-m365-mail-sec.png)

   - **名称**：同意请求审批者

    ![显示用户正在管理中心为组提供"同意请求审批者"Microsoft 365屏幕截图。](images/data-connect-m365-cons-apprv.png)

   - **Email Prefix**： consentrequestapprovers

    ![Screenshot showing a user creating the email address for the previously created group in the Microsoft 365 admin center.](images/data-connect-m365-cons-apprv-pref.png)

1. **新创建的组** 最多可能需要一个小时才能显示在列表中。 创建组后，选择它。

1. 再次转到 **活动组** 选项，然后搜索你刚刚创建的组。

1. 选择组，在"成员 **"** 选项卡中，选择"**查看所有和管理成员"。**

1. 将启用全局管理员角色 **的两个用户** 添加到此新组中。

## <a name="enable-microsoft-graph-data-connect-in-your-microsoft-365-tenant"></a>在 Graph 租户中连接 Microsoft Microsoft 365 Data Microsoft 365

在此步骤中，你将在 Graph 租户连接 Microsoft Microsoft 365 服务。

1. 当你仍登录到管理门户Microsoft 365，选择 **"设置 >""组织设置"** 菜单项。

1. 选择 **Microsoft Graph Data 连接** 服务。

    ![显示"组织设置"边栏选项卡中的"服务"的屏幕截图。 用户正在切换 Microsoft Graph管理连接 Microsoft Microsoft 365 服务。](images/data-connect-m365-mgdc-toggle.png)

1. 选中显示为整个组织打开或Graph Microsoft 连接"复选框 **以** 启用数据连接。

    ![显示为整个组织启用数据记录功能而必须连接复选框的屏幕截图。](images/data-connect-m365-enable-mgdc-for-org.png)

1. 输入 **同意请求** (或你之前创建的组的名称) 在用户组中做出审批决定，**然后选择保存。** 
