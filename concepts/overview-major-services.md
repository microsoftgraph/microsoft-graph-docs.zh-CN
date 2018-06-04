# <a name="major-services-and-features-in-microsoft-graph"></a>Microsoft Graph 中的主要服务和功能

Microsoft Graph 使你可以与 Office 365、Windows 10 以及 Microsoft 365 中的企业移动性与安全性服务充分集成。 此外，它提供安全性和社交智能，可以提高用户的工作效率、创造性和团队协作，并保护企业资源和用户数据。 

## <a name="users-and-groups"></a>用户和组

Microsoft Graph 的核心是用户和组的概念。 

Microsoft Graph 中的_用户_是数以百万计使用 Microsoft 365 云服务的用户之一。 它是身份受到保护且访问得到妥善管理的焦点。 用户数据是业务发展的驱动力。 Microsoft Graph 服务可将这些数据提供给企业，在丰富的环境中、实时更新和深度见解中，并且始终仅在适当的权限下使用这些数据。

Office 365 _组_是允许用户进行协作的基本实体。 它与其他服务集成，在任务规划、团队合作、教育等方面提供更丰富的方案。 

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 用户 | Azure AD 和大多数高效工作、协作、智能和教育服务 | 用户是 Microsoft Graph 的核心重点，Microsoft Graph 服务围绕这一点构建以用户为中心的功能。 | [Microsoft Graph 中的用户概述](../concepts/azuread-users-concept-overview.md)|
|组 | Azure AD、OneDrive、OneNote、Outlook、Planner | Office 365 组为用户提供了基本协作单元，以共享对话、文件、笔记、日历和计划等。 | [Microsoft Graph 中的 Office 365 组概述](../concepts/office365-groups-concept-overview.md) |

## <a name="connecting-users-data-microsoft-365-services-and-your-apps"></a>连接用户数据、Microsoft 365 服务和你的应用

从核心用户和组开始，Microsoft Graph 构建了一个 Microsoft 365 服务和功能网络，用于管理、保护和提取数据，以支持各种各样的场景。 Microsoft Graph 允许你在始终尊从适当授权的情况下访问这些大量的用户数据。

![Microsoft Graph 将你连接到用户数据](images/microsoft-graph-connects-users-data.png)

### <a name="services-and-features"></a>服务和功能

Microsoft Graph 中的一些服务是首次推出，其他服务则是我们所熟知的独立服务且目前融入 Microsoft Graph 中。 它们的 API 集遵循 [Microsoft REST API 准则](https://github.com/Microsoft/api-guidelines)中详述的简化设计，现在可通过单个 Microsoft Graph REST 终结点 `https://graph.microsoft.com` 进行访问。 本文其余部分按类别列出了主要服务和功能。 


## <a name="identity-and-access-management"></a>标识和访问管理

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 标识和访问管理 | Azure AD | 创建和管理目录资源，如用户、组和应用程序。 管理对资源和数据的访问。 | [Azure AD 标识和访问管理概述](../concepts/azuread-identity-access-management-concept-overview.md)  |


## <a name="productivity"></a>工作效率

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 日历 | Outlook  | 允许用户在 Web、移动和桌面设备上设置约会和会议。 它是 Office 365 中 Outlook 消息传递通信中心的一部分，还允许用户管理电子邮件和联系人。 | [Outlook 日历概述](../concepts/outlook-calendar-concept-overview.md)  |
| 文件 | OneDrive 和 SharePoint | 在 OneDrive 和 SharePoint 上管理和共享用户文件。 | [OneDrive 文件存储概述](../concepts/onedrive-concept-overview.md) |
| 邮件 | Outlook | 允许用户在 Web、移动和桌面设备上进行通信、组织邮件，并管理其工作流中的优先事项。 它是 Office 365 中 Outlook 通信中心的一部分，还允许用户管理联系人和安排会议。 | [Outlook 邮件概述](../concepts/outlook-mail-concept-overview.md) |
| 笔记 | OneNote | 允许用户规划和组织观点及信息。 | [OneNote 笔记概述](../concepts/integrate_with_onenote.md) |
| 个人联系人 | Outlook | Web、移动和桌面设备上的联系人管理器。 它是 Office 365 中 Outlook 消息传递通信中心的一部分，还允许用户管理电子邮件和安排会议。  | [Outlook 个人联系人概述](../concepts/outlook-contacts-concept-overview.md) |
| 工作簿和图表 | Excel | 允许用户使用 Excel 电子表格进行复杂计算、跟踪、分析和可视化数据，并生成专业报表。 | [Excel 工作簿和图表概述](../concepts/excel-concept-overview.md) |


## <a name="collaboration"></a>协作

<!-- Want to update links to concept overviews as they are created over time. 
-->
|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 站点和列表  | SharePoint | 面向用户和 Office 365 组的基于 Web 的平台，以共享、组织、管理和发现内容（包括列表、文件和笔记）。 | [SharePoint 网站和内容概述](../concepts/sharepoint-concept-overview.md) | 
|任务和计划 | Planner | 使 Office 365 组中的用户能够创建计划、分配任务和跟踪进度。 | [Planner 计划和任务概述](../concepts/planner-concept-overview.md) |
|团队合作（预览） |  Microsoft Teams | 面向团队的数字中心和基于聊天的工作区，用于共享文件、笔记、日历和计划。 | [Microsoft Teams 团队合作概述](../concepts/teams-concept-overview.md) |


## <a name="social-intelligence-and-analytics"></a>社交智能和分析

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 社交智能：人员 | Azure AD、Outlook、SharePoint 等 | 获取有关人员的信息，该对象按与用户的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。  | [Microsoft Graph 中的社交智能](../concepts/social-intel-concept-overview.md) |
| 社交智能：文档见解（预览） | Delve、OneDrive、Outlook、SharePoint | 使用高级分析和机器学习技术获取常用的文档，以及用户查看、修改或共享的文档。  | [Microsoft Graph 中的社交智能](../concepts/social-intel-concept-overview.md)  |


## <a name="device-management"></a>设备管理

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
|设备和应用 | Intune | 注册和配置设备，并管理组织中的移动应用程序。 | [Intune 设备和应用概述](../concepts/intune-concept-overview.md) |


## <a name="security"></a>安全性

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 安全集成（预览） | Azure AD Identity Protection、Azure 安全中心 | 在整个 Microsoft 和生态系统合作伙伴中提供安全见解和操作的统一网关。 | [Microsoft Graph 中的安全性](../concepts/security-concept-overview.md) |
| Identity Protection（预览） | Azure AD | 在 Azure AD 中为用户提供对登录和帐户风险数据的访问。 | [Microsoft Graph 中的安全性](../concepts/security-concept-overview.md)  |



## <a name="cross-device-experiences"></a>跨设备体验

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 跨设备体验 | 活动源、设备中继 | 支持超越单一设备的应用体验，同用户在不同设备之间移动，而不考虑设备类型和平台。 | [跨设备体验概述](../concepts/cross-device-concept-overview.md) |


## <a name="usage-reports"></a>使用率报告

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 报告 | Microsoft Teams、OneDrive、Outlook、SharePoint、Skype for Business、Yammer | 获取支持服务的活动和用法信息。 | [使用情况报表概述](../concepts/reportroot-concept-overview.md) |


## <a name="education"></a>教育

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 教育 | Azure AD、教育 | 提供了与教育场景相关的信息，包括学校、课堂、学生、教师和作业信息。 支持 ISV 构建面向教室的应用程序，从而节约教师时间并提升团队合作与协作。  | [教育概述](../concepts/education-concept-overview.md) |


## <a name="business-applications"></a>业务应用程序

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 客户预订（预览） | Microsoft Bookings | 针对小型企业，使其客户可以直接在 Web 或 Facebook 上预定服务。 让业务运营商管理客户偏好、服务和定价、员工列表和日程安排，以及其他常见的业务信息。 | [Microsoft Bookings API 概述](../concepts/booking-concept-overview.md) |


## <a name="next-steps"></a>后续步骤

<!-- Need to update the destination page titles and URLs as Matt's v-team finalize on the examples and featured scenarios content 
-->

- 请参阅基于 Microsoft Graph 服务构建的创造性解决方案[示例](https://developer.microsoft.com/zh-CN/graph/examples)，可帮助解决实际客户问题。
- 在目录的**了解**部分，阅读有关_你_可在应用场景中使用的服务和功能。
- 尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的示例请求。
- 使用[快速入门](https://developer.microsoft.com/graph/quick-start)设置一个即可运行的示例应用。