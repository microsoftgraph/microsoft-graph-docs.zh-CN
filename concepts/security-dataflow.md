# <a name="microsoft-graph-security-data-flow"></a>Microsoft Graph Security 数据流

Microsoft Graph Security API 建立联盟与 Microsoft Graph Security 生态系统中的所有提供商的请求。 这基于应用程序提供的安全提供程序同意，如下图所示。 同意工作流仅适用于非 Microsoft 提供程序。

![security_dataflow_1.png](./images/security_dataflow_1.png)

以下是流程的说明：

1. 应用程序用户登录到要查看从提供程序的同意窗体的提供程序应用程序。 此同意表单体验或 UI 由提供程序拥有，仅适用于非 Microsoft 提供程序，以从客户那里获得发送请求给 Microsoft Graph Security API 的明确同意。
2. 客户端同意存储在提供程序侧。
3. 提供程序 consent 服务调用 Microsoft Graph Security API，告知各自客户同意审批。
4. 应用程序将请求发送到 Microsoft Graph Security API。
5. Microsoft Graph Security API 检查映射到不同提供程序的此客户同意信息。
6. Microsoft Graph Security API 调用客户通过提供程序同意体验提供明确同意的所有这些提供程序。
7. 响应从该客户端的所有已同意提供程序返回。
8. 结果集响应返回到应用程序。
9. 如果客户未同意任何提供程序，则响应不包含这些提供程序的任何结果。
