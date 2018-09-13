# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>使用 Microsoft Graph 中的通知数 API 启用以人为本的通知体验 

通知是重新找回用户的最有效方式。 它们可以捕获用户的注意，并将用户重新带回应用。 在多设备世界中，用户可以从任何位置、在跨安装有应用的不同平台和设备上访问应用。 

应该采用“以人为本”的方式设计通知方案，不论用户是男还是女，这种设计方式的主要目标是通知用户。 现有的主要平台提供的通知解决方案在面向目标设备方面是极好的。 Microsoft Graph 通知数允许针对目标用户，进一步扩大了这方面的优势。 Microsoft Graph 通知数将会照顾到繁重的工作内容，包括用户和端点之间的映射、同步跨用户不同端点的通知状态等。 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>为什么要集成 Microsoft Graph 通知数？
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>向跨不同端点的用户发送通知
作为 Microsoft Graph 的组成部分，通知数 API 允许针对某个 Microsoft 帐户或某个工作或学校 (Azure AD) 帐户发送通知。 平台将此通知分发到所有用户的端点，包括 Windows UWP 、 Android 以及 iOS 。 

### <a name="manage-notifications-across-endpoints"></a>跨端点管理通知数
Microsoft Graph 通知数 API 允许更新通知的状态并将此状态同步至所有端点。 例如，当用户在一个设备上对通知作出反应时，则可以更新此通知的状态 （例如，将其标记为已读或已解除），此相同的状态更改将分发给所有其他端点。 Microsoft Graph 通知数 API 用一种集中方式跟踪用户的通知数状态，这样便于确保通知数被处理一次，并解除所有端点。

### <a name="retrieve-notification-history"></a>检索通知历史记录
可以按照定义的到期时间（最多 30 天），用通知数 API 检索通知历史记录。 在历史记录中仍然可以检索到标记为已读或已解除的通知，启用应用内的通知历史记录视图和其他方案。 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>与 Microsoft Graph 中的通知数 API 集成

只需简单的几个步骤便可以将应用与 Microsoft Graph 通知数集成 - 通过 Windows Dev Center 加载应用，使用 [创建通知](../api-reference/beta/api/projectrome_notification_post.md) 方法发布通知数，在应用客户端使用 Project Rome SDK 接收和管理通知数。  

若要了解有关如何通过 Microsoft Graph 发布用户通知数的详细信息，请参阅 [通知数 API 参考](../api-reference/beta/resources/notifications-api-overview.md) 。
 
若要了解有关通过与 Project Rome SDK 集成，接收和管理通知数的详细信息，请参阅 [Project Rome SDK 文档](https://docs.microsoft.com/en-us/windows/project-rome/) 

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的跨设备体验](cross-device-concept-overview.md)
- [Project Rome Dev Center](http://aka.ms/projectrome)
