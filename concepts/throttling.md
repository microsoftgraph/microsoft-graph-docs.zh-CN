# <a name="microsoft-graph-throttling-guidance"></a>Microsoft Graph 限制指南


限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。

根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。

## <a name="what-happens-when-throttling-occurs"></a>在限制时，会发生什么情况？

超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。 

## <a name="common-throttling-scenarios"></a>常见的限制场景

客户端受限的最常见原因包括：

* 来自租户中所有应用程序的请求太多。
* 来自所有租户中特定应用程序的请求太多。

## <a name="best-practices-to-handle-throttling"></a>处理限制的最佳实践

以下是处理限制的最佳做法：

* 减少每个请求的操作数量。
* 减少调用频率。
* 避免立即重试，因为所有请求都会计入使用限制。

进行错误处理时，使用 HTTP 错误代码 429 检测限制。 失败响应的响应头中有“重试间隔”**字段。 使用*重试间隔*延迟回退请求是从限制中恢复的最快速方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。

1. 等待“重试间隔”**字段中指定的秒数。
2. 重试请求。
3. 如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的重试间隔延迟并重试请求直到成功。

下列资源目前提供“重试间隔”头：
- [用户](../api-reference/v1.0/resources/user.md)
- [照片](../api-reference/v1.0/resources/profilephoto.md)
- [邮件](../api-reference/v1.0/resources/message.md)
- [日历（用户和组）](../api-reference/v1.0/resources/event.md)
- [联系人](../api-reference/v1.0/resources/contact.md)
- [附件](../api-reference/v1.0/resources/attachment.md)
- [组对话](../api-reference/v1.0/resources/conversation.md)
- [人员和社交活动](../api-reference/beta/resources/social_overview.md)
- [Drive (OneDrive)](../api-reference/v1.0/resources/drive.md)

有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://msdn.microsoft.com/zh-CN/library/office/dn589798.aspx)。
