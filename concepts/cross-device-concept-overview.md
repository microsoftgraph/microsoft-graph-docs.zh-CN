# <a name="cross-device-experiences-in-microsoft-graph"></a>Microsoft Graph 中的跨设备体验

在当今的多设备环境中，消费者使用设备的方式跨越了不同的平台和外形规格：他们可能会在其平板电脑上阅读早间新闻，在早晨上班途中用手机查看电子邮件，以及在工作时使用台式电脑。 到了晚上，他们可能会在自己的家庭媒体控制台上观看电影，并使用智能扬声器获取当天的新闻。 一般客户全天会使用多个设备和平台。 

在过去，外形规格会造成消费者之间不同类型的行为差异。 然而，今天，多设备消费者可在他们的所有设备上进行所有活动。 每天（无论是在家中与家人一起，还是在工作时与同事一起）执行的任务本质上不是以设备为中心的，而是**以人为中心的**。 消费者希望能够使用任何可用的屏幕，而不管输入来自何处。 事实上，他们通常发现每台设备都有一个清晰的边界，并且跨设备完成任务需要非自然的操作，例如向自己发送电子邮件或使用 U 盘。 客户在其设备之间移动时会遇到冲突，有时由于这种环境切换，重要的任务会丢失。 这对开发者而言同样是一个挑战，因为当客户使用应用感到摩擦时，客户就会对该应用的参与度会下降。

Microsoft 正在构建一个平台，以打造超越单一设备的体验，以便他们能够跨设备进行协调，让你能够创建**以人为中心的**可与用户一起移动的应用场景，并模糊其设备之间的界限，而不考虑外形规格或平台。 Microsoft Graph 提供了单个统一的终结点，让你可以访问 Azure Active Directory 和 Office 365 中的数据。 现在，通过 Microsoft Graph，你还可以访问属于你客户的活动和设备，并实现跨设备和平台的以人为中心的丰富体验。 

## <a name="why-invest-in-cross-device-experiences"></a>为何要投资跨设备体验？

### <a name="let-customers-pick-up-where-they-leave-off-with-the-activity-feed-api"></a>让客户通过活动源 API 获取他们离开的位置 
通过活动，你可以为在任何平台和设备上无缝流动的应用用户捕获独特任务，从而使他们能够在其首选屏幕上快速恢复工作。 使用活动源，你可以创建对用户最重要的、以人为中心的任务视图，帮助减少从网页切换到移动设备再到个人电脑等设备时的阻碍。 

### <a name="build-rich-cross-device-experiences-by-using-the-device-relay-api"></a>通过使用设备中继 API 构建丰富的跨设备体验 
除了 Microsoft 设备（个人电脑、Windows Phone、Xbox、IoT、HoloLens 等），设备中继 API 还提供了 Android 和 iOS 设备。 这可让能够真正打破用户设备之间的边界。 你可以构建利用用户环境的应用，并创建能够实时超越单个设备的丰富体验。 

## <a name="reach-out-to-and-engage-with-users-anywhere-via-a-coherent-and-human-centric-notification-story-preview"></a>通过以人为文本的一致通知故事（预览版），接触用户并与之接洽

通知是与用户沟通和接洽最有效和直接的方式之一。 

利用 Microsoft Graph 通知 API，你可以采用以人为本（而不是以设备为中心）的方式传递通知。 你可以针对将接收通知的用户，并依赖于 Microsoft Graph 通知框架将通知传递到用户登录到的每个端点。 利用 Microsoft Graph 通知 API 也可以轻松地完成跨设备通知管理，因此你可以跨用户的设备同步通知，让用户不再执行多余的工作，并且不会中断用户的工作。 

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft Graph API 实现跨设备体验](../api-reference/v1.0/resources/cross-device-reference-overview.md)
- [详细了解 Microsoft Graph 中的活动源 API](activity-feed-concept-overview.md)
- [详细了解 Microsoft Graph 中的设备重播 API](device-relay-concept-overview.md)
- [详细了解 Microsoft Graph 中的 Microsoft Graph 通知 API](notifications-concept-overview.md)
