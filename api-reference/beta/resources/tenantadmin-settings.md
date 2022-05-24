---
title: 设置资源类型
description: 表示SharePoint和OneDrive的租户级别设置。
author: liamfernandez
ms.localizationpriority: medium
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: acc37088c339abeaf0e6405e00ef45a344803e9c
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653611"
---
# <a name="settings-resource-type"></a>设置资源类型
命名空间：microsoft.graph.tenantAdmin

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示SharePoint和OneDrive的租户级别设置。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明
|:---|:---|:---
|[获取设置](../api/tenantadmin-settings-get.md)|[microsoft.graph.tenantAdmin.settings](../resources/tenantadmin-settings.md) | 获取SharePoint和OneDrive的租户级别设置。|
|[更新设置](../api/tenantadmin-settings-update.md) | [microsoft.graph.tenantAdmin.settings](../resources/tenantadmin-settings.md) | 更新SharePoint和OneDrive的一个或多个租户级别设置。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| allowedDomainGuidsForSyncApp                       | GUID 集合              | OneDrive 同步应用的受信任域 GUID 的集合。                                                                                                                                                  |
| availableManagedPathsForSiteCreation               | String collection            | 可用于网站创建的托管路径的集合。 只读。                                                                                                                                            |
| deletedUserPersonalSiteRetentionPeriodInDays       | Int32                        | 保留已删除用户OneDrive的天数。                                                                                                                                                   |
| excludedFileExtensionsForSyncApp                   | String collection            | OneDrive 同步应用未上传的文件扩展名的集合。                                                                                                                                           |
| imageTaggingOption                                 | [tenantAdmin.imageTaggingChoice](../resources/tenantadmin-settings.md#imagetaggingchoice-values)           | 指定租户的图像标记选项。 可取值为：`disabled`、`basic`、`enhanced`。                                                                                                       |
| isCommentingOnSitePagesEnabled                     | Boolean                      | 指示是否允许在SharePoint的新式网站页面上使用注释。                                                                                                                                          |
| isFileActivityNotificationEnabled                  | Boolean                      | 指示是否为OneDrive事件启用推送通知。                                                                                                                                               |
| isLoopEnabled                                      | Boolean                      | 指示是否允许在SharePoint网站上Fluid Framework。                                                                                                                                                   |
| isMacSyncAppEnabled                                | Boolean                      | 指示是否可以使用适用于 Mac 的OneDrive 同步应用同步文件。                                                                                                                                          |
| isResharingByExternalUsersEnabled                  | Boolean                      | 指示是否允许来宾重新共享他们不拥有的文件、文件夹和网站。                                                                                                                           |
| isSharePointMobileNotificationEnabled              | Boolean                      | 指示是否为SharePoint启用了移动推送通知。                                                                                                                                             |
| isSharePointNewsfeedEnabled                        | Boolean                      | 指示是否允许在SharePoint的新式网站页面上使用新闻源。                                                                                                                                   |
| isSiteCreationEnabled                              | Boolean                      | 指示是否允许用户创建网站。                                                                                                                                                           |
| isSiteCreationUIEnabled                            | Boolean                      | 指示是否显示用于创建网站的 UI 命令。                                                                                                                                                     |
| isSitePagesCreationEnabled                         | Boolean                      | 指示是否允许在SharePoint网站上创建新的新式页面。                                                                                                                                         |
| isSitesStorageLimitAutomatic                       | Boolean                      | 指示站点存储空间是自动管理的还是每个站点是否设置了特定的存储限制。                                                                                                       |
| isSyncButtonHiddenOnPersonalSite                   | Boolean                      | 指示是否隐藏OneDrive中的同步按钮。                                                                                                                                                            |
| isUnmanagedSyncAppForTenantRestricted              | Boolean                      | 指示是否允许用户仅在已加入特定域的电脑上同步文件。                                                                                                                           |
| personalSiteDefaultStorageLimitInMB                | Int64                        | 为所有分配了限定许可证的新用户和现有用户的默认OneDrive存储限制。 以兆字节为单位 (MB) 。                                                                           |
| sharingAllowedDomainList                           | String collection            | 允许在组织外部共享的电子邮件域的集合。                                                                                                                              |
| sharingBlockedDomainList                           | String collection            | 阻止在组织外部共享的电子邮件域的集合。                                                                                                                              |
| sharingCapability                                  | [tenantAdmin.sharingCapabilities](#sharingcapabilities-values)          | 租户的共享功能。 可能的值是：`disabled`、`externalUserSharingOnly`、`externalUserAndGuestSharing`、`existingExternalUserSharingOnly`。                                                |
| sharingDomainRestrictionMode                       | [tenantAdmin.sharingDomainRestrictionMode](#sharingdomainrestrictionmode-values) | 指定域的外部共享模式。 可取值为：`none`、`allowList`、`blockList`。                                                                                                        |
| siteCreationDefaultManagedPath                     | String                       | 团队网站托管路径的值。 这是创建新团队网站的路径。                                                                                                          |
| siteCreationDefaultStorageLimitInMB                | Int32                        | 创建新站点时的默认存储配额。 以兆字节为单位 (MB) 。                                                                                                                            |
| tenantDefaultTimezone                              | String                       | 新创建的站点的租户的默认时区。                                                                                                                                                      |

### <a name="imagetaggingchoice-values"></a>imageTaggingChoice 值
| 成员                          | 说明                                                                                                           |
| :------------------------------ | :---------------------------------------------------------------------------------------------------------------------|
| 禁用                        | 已禁用租户的图像标记选项。                                                                  |
| 基本                           | 允许租户中的用户向图像添加基本标记，以便通过搜索访问它们。                    |
| 增强                        | 允许用户使用自定义标记和增强功能标记图像。                                                    |
| unknownFutureValue              | 可变枚举 sentinel 值。 请勿使用。                                                                     |

### <a name="sharingcapabilities-values"></a>sharingCapabilities 值
| 成员                          | 说明                                                                                                           |
| :------------------------------ | :---------------------------------------------------------------------------------------------------------------------|
| 禁用                        | 用户只能与组织中的人员共享。 不允许外部共享。                                 |
| externalUserSharingOnly         | 用户可以与新来宾和现有来宾共享。 来宾必须登录或提供验证码。                     |
| externalUserAndGuestSharing     | 用户可以使用不需要登录的链接与任何人共享。                                                |
| existingExternalUserSharingOnly | 用户可以与现有来宾共享 (组织) 目录中已有的来宾。                            |
| unknownFutureValue              | 可变枚举 sentinel 值。 请勿使用。                                                                     |

### <a name="sharingdomainrestrictionmode-values"></a>sharingDomainRestrictionMode 值
| 成员                          | 说明                                                                                                           |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| 无                            | 不适用任何限制。                                                                                                |
| allowList                       | 用户将能够与仅来自允许的电子邮件域列表的外部协作者共享。           |
| blockList                       | 除了被阻止的电子邮件域列表中的外部协作者之外，用户将能够与所有外部协作者共享。 |
| unknownFutureValue              | 可变枚举 sentinel 值。 请勿使用。                                                                     |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.tenantAdmin.settings",
  "openType": "false"
}
-->
``` json
{
    "allowedDomainGuidsForSyncApp": ["string (identifier)"],
    "availableManagedPathsForSiteCreation": ["string"],
    "deletedUserPersonalSiteRetentionPeriodInDays": "Int32",
    "excludedFileExtensionsForSyncApp": ["string"],
    "id": "string (identifier)",
    "imageTaggingOption": "string",
    "isCommentingOnSitePagesEnabled": "boolean",
    "isFileActivityNotificationEnabled": "boolean",
    "isLoopEnabled": "boolean",
    "isMacSyncAppEnabled": "boolean",
    "isResharingByExternalUsersEnabled": "boolean",
    "isSharePointMobileNotificationEnabled": "boolean",
    "isSharePointNewsfeedEnabled": "boolean",
    "isSiteCreationEnabled": "boolean",
    "isSiteCreationUIEnabled": "boolean",
    "isSitePagesCreationEnabled": "boolean",
    "isSitesStorageLimitAutomatic": "boolean",
    "isSyncButtonHiddenOnPersonalSite": "boolean",
    "isUnmanagedSyncAppForTenantRestricted": "boolean",
    "personalSiteDefaultStorageLimitInMB": "Int64",
    "sharingAllowedDomainList" : ["string"],
    "sharingBlockedDomainList" : ["string"],
    "sharingCapability": "string",
    "sharingDomainRestrictionMode": "string",
    "siteCreationDefaultManagedPath": "string",
    "siteCreationDefaultStorageLimitInMB": "Int32",
    "tenantDefaultTimezone": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "settings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "namespace": "microsoft.graph.tenantAdmin"
}
-->
