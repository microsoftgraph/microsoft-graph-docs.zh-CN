---
title: educationSynchronizationProfile 资源类型
description: 表示一组用于将源目录中的教育实体和名单信息同步到 Azure Active Directory (Azure AD) 的配置。 此资源提供在学校数据同步中使用的编程表示形式。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2db53346ae270f5441637835ec5da0427d9d4ab8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989596"
---
# <a name="educationsynchronizationprofile-resource-type"></a>educationSynchronizationProfile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一组用于将源目录中的教育实体和名单信息同步到 Azure Active Directory (Azure AD) 的配置。 此资源提供在 [学校数据同步](https://sds.microsoft.com)中使用的编程表示形式。

## <a name="methods"></a>方法

| 方法                                                                    | 返回类型                                                 | 说明                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [列出配置文件](../api/educationsynchronizationprofile-list.md)           | [educationSynchronizationProfile] 集合                | 获取租户中所有同步配置文件的列表。                                                                  |
| [获取个人资料](../api/educationsynchronizationprofile-get.md)              | [educationSynchronizationProfile]                           | 在给定配置文件标识符的情况检索特定配置文件。                                                                      |
| [创建配置文件](../api/educationsynchronizationprofile-post.md)          | 无                                                        | 创建新的同步配置文件。                                                                                          |
| [删除个人资料](../api/educationsynchronizationprofile-delete.md)        | [educationSynchronizationProfile]                           | 在给定配置文件标识符的情况删除特定配置文件。                                                                        |
| [暂停配置文件](../api/educationsynchronizationprofile-pause.md)          | 无                                                        | 暂停正在进行的同步。                                                                                              |
| [恢复配置文件](../api/educationsynchronizationprofile-resume.md)        | 无                                                        | 恢复暂停的同步。                                                                                               |
| [重置配置文件](../api/educationsynchronizationprofile-reset.md)          | 无                                                        | 重置配置文件的状态并重新启动同步。                                                                    |
| [启动 CSV 配置文件](../api/educationsynchronizationprofile-start.md)      | [educationFileSynchronizationVerificationMessage]集合 | 验证上载的源文件并启动同步。 仅在数据提供程序为 [educationCsvDataProvider]时适用。 |
| [获取 CSV 上载 URL](../api/educationsynchronizationprofile-uploadurl.md) | 字符串                                                      | 返回短生存期的 URL 以上载 CSV 数据文件。 仅在数据提供程序为 [educationCsvDataProvider]时适用。        |
| [获取状态](../api/educationsynchronizationprofilestatus-get.md)         | [educationsynchronizationProfileStatus]                     | 返回特定同步配置文件的状态。                                                                       |
| [获取错误](../api/educationsynchronizationerrors-get.md)                | [educationSynchronizationError] 集合                  | 获取同步过程中生成的所有错误。                                                                           |

## <a name="properties"></a>属性

| 属性                             | 类型                                                   | 说明                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| id                                   | String                                                 | 资源的唯一标识符。  (只读)                                                                                |
| displayName                          | String                                                 | 用于同步标识的配置文件的名称。                                                                         |
| dataProvider                         | [educationSynchronizationDataProvider]                 | 用于配置文件的数据提供程序。                                                                                           |
| expirationDate                       | 日期                                                   | 应将配置文件视为已过期并停止同步的日期。 When `null` 。 配置文件永远不会过期。 （可选）       |
| handleSpecialCharacterConstraint     | Bool                                                   | 确定在从源同步时，学校数据同步是否应自动替换不受支持的特殊字符。             |
| identitySynchronizationConfiguration | [educationIdentitySynchronizationConfiguration]        | 确定配置文件应如何 [新建][fullsync] 或 [匹配现有][dirsync] AAD 用户。                                  |
| licensesToAssign                     | [educationSynchronizationLicenseAssignment] 集合 | 许可证安装程序配置。                                                                                                      |
| state                                | educationSynchronizationProfileState                   | 配置文件的状态。 可取值为：`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed`。 |

## <a name="relationships"></a>关系

| 关系  | 类型                                       | 说明                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| 错误        | [educationSynchronizationError] 集合 | 与此同步配置文件关联的所有错误。 |
| profileStatus | [educationSynchronizationProfileStatus]    | 同步状态。                              |

## <a name="data-providers"></a>数据提供程序

每个 [educationSynchronizationProfile] 必须指定要用作同步源的以下数据提供程序之一。

| Data Provider                                                             | 说明                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [educationCsvDataProvider]                                                | 上载到配置文件的[SAS URL](../api/educationsynchronizationprofile-uploadurl.md)的 CSV 文件 |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | OneRoster v1.1 API                                                                                 |
| [educationPowerSchoolDataProvider]                                        | PowerSchool API                                                                                    |

## <a name="json-representation"></a>JSON 表示形式

下面是 **educationSynchronizationProfile** 资源的 JSON 表示形式。

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
  "suppressions": [
      "Error: microsoft.graph.educationSynchronizationProfile/dataProvider:\r\n      Referenced type microsoft.graph.educationSynchronizationDataProvider is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->


