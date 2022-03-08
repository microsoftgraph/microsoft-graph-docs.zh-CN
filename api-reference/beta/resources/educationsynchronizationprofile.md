---
title: educationSynchronizationProfile 资源类型
description: 表示一组用于将教育实体和名单信息从源目录同步到Azure Active Directory (Azure AD) 。 此资源提供在资源中使用的编程学校数据同步。
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e3b687e3856ae8d7805bf4b74724c70380359a9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336002"
---
# <a name="educationsynchronizationprofile-resource-type"></a>educationSynchronizationProfile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一组用于将教育实体和名单信息从源目录同步到Azure Active Directory (Azure AD) 。 此资源提供在资源中使用的编程[学校数据同步](https://sds.microsoft.com)。

## <a name="methods"></a>方法

| 方法                                                                    | 返回类型                                                 | 说明                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [列出配置文件](../api/educationsynchronizationprofile-list.md)           | [educationSynchronizationProfile] 集合                | 获取租户中所有同步配置文件的列表。                                                                  |
| [获取个人资料](../api/educationsynchronizationprofile-get.md)              | [educationSynchronizationProfile]                           | 检索给定配置文件标识符的特定配置文件。                                                                      |
| [创建配置文件](../api/educationsynchronizationprofile-post.md)          | 无                                                        | 创建新的同步配置文件。                                                                                          |
| [删除个人资料](../api/educationsynchronizationprofile-delete.md)        | [educationSynchronizationProfile]                           | 删除给定配置文件标识符的特定配置文件。                                                                        |
| [暂停配置文件](../api/educationsynchronizationprofile-pause.md)          | 无                                                        | 暂停正在进行的同步。                                                                                              |
| [恢复配置文件](../api/educationsynchronizationprofile-resume.md)        | 无                                                        | 恢复暂停的同步。                                                                                               |
| [重置配置文件](../api/educationsynchronizationprofile-reset.md)          | 无                                                        | 重置配置文件的状态并重新启动同步。                                                                    |
| [启动 CSV 配置文件](../api/educationsynchronizationprofile-start.md)      | [educationFileSynchronizationVerificationMessagecollection] | 验证上载的源文件并开始同步。 仅适用于数据提供程序为 [educationCsvDataProvider 的情况]。 |
| [获取 CSV 上传 URL](../api/educationsynchronizationprofile-uploadurl.md) | string                                                      | 返回用于上载 CSV 数据文件的短期 URL。 仅适用于数据提供程序为 [educationCsvDataProvider 的情况]。        |
| [获取状态](../api/educationsynchronizationprofilestatus-get.md)         | [educationsynchronizationProfileStatus]                     | 返回特定同步配置文件的状态。                                                                       |
| [获取错误](../api/educationsynchronizationerrors-get.md)                | [educationSynchronizationError] 集合                  | 获取同步期间生成的所有错误。                                                                           |

## <a name="properties"></a>属性

| 属性                             | 类型                                                   | 说明                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| id                                   | String                                                 | 资源的唯一标识符。  (只读)                                                                                |
| displayName                          | 字符串                                                 | 用于同步标识的配置文件的名称。                                                                         |
| dataProvider                         | [educationSynchronizationDataProvider]                 | 用于配置文件的数据提供程序。                                                                                           |
| expirationDate                       | Date                                                   | 将配置文件视为已过期并停止同步的日期。 `YYYY-MM-DD`按照 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) 的格式提供日期。 最大值为自配置文件创建起 18 个月。  （可选）       |
| handleSpecialCharacterConstraint     | Bool                                                   | 确定是否在学校数据同步源同步时自动替换不受支持的特殊字符。             |
| identitySynchronizationConfiguration | [educationIdentitySynchronizationConfiguration]        | 确定配置文件应[如何新建或][fullsync][匹配现有AAD][dirsync]用户。                                  |
| licensesToAssign                     | [educationSynchronizationLicenseAssignment] 集合 | 许可证设置配置。                                                                                                      |
| state                                | educationSynchronizationProfileState                   | 配置文件的状态。 可取值为：`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed`。 |

## <a name="relationships"></a>关系

| 关系  | 类型                                       | 说明                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| 错误        | [educationSynchronizationError] 集合 | 与此同步配置文件关联的所有错误。 |
| profileStatus | [educationSynchronizationProfileStatus]    | 同步状态。                              |

## <a name="data-providers"></a>数据提供程序

每个 [educationSynchronizationProfile] 必须指定一个要用作同步源的以下数据提供程序。

| Data Provider                                                             | 说明                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [educationCsvDataProvider]                                                | 上传到配置文件的 [SAS URL 的 CSV 文件](../api/educationsynchronizationprofile-uploadurl.md) |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | OneRoster v1.1 API                                                                                 |
| [educationPowerSchoolDataProvider]                                        | PowerSchool API                                                                                    |

## <a name="json-representation"></a>JSON 表示形式

以下是 **educationSynchronizationProfile** 资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "state": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileState"
  },
  "profileStatus": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
  },
  "errors": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
    }
  ],
  "dataProvider": {
    "@odata.type": "microsoft.graph.educationCsvDataProvider"
  },
  "identitySynchronizationConfiguration": {
    "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
  },
  "licensesToAssign": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
    }
  ],
  "handleSpecialCharacterConstraint": "Boolean",
  "expirationDate": "Date"
}
```

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationsynchronizationprofilestatus]: educationsynchronizationProfileStatus.md
[educationsynchronizationerror]: educationSynchronizationError.md
[educationfilesynchronizationverificationmessage]: educationFileSynchronizationVerificationMessage.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationidentitysynchronizationconfiguration]: educationIdentitySynchronizationConfiguration.md
[educationsynchronizationlicenseassignment]: educationSynchronizationLicenseAssignment.md
[fullsync]: educationidentitycreationconfiguration.md
[dirsync]: educationidentitycreationconfiguration.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSynchronizationProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
}-->


