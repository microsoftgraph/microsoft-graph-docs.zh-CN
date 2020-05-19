---
title: educationSynchronizationProfile 资源类型
description: 表示一组用于将源目录中的教育实体和名单信息同步到 Azure Active Directory （Azure AD）的配置。 此资源提供在学校数据同步中使用的编程表示形式。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c498abb711a336f3627ef0b63e6c742e633ea05a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289933"
---
# <a name="educationsynchronizationprofile-resource-type"></a>educationSynchronizationProfile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一组用于将源目录中的教育实体和名单信息同步到 Azure Active Directory （Azure AD）的配置。 此资源提供在[学校数据同步](https://sds.microsoft.com)中使用的编程表示形式。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-|:-|:-|
| [列出同步配置文件](../api/educationsynchronizationprofile-list.md) | **educationSynchronizationProfile**集合 | 获取租户中所有同步配置文件的列表。 |
| [获取同步配置文件](../api/educationsynchronizationprofile-get.md) | **educationSynchronizationProfile** | 在给定配置文件标识符的情况检索特定配置文件。 |
| [创建同步配置文件](../api/educationsynchronizationprofile-post.md) | 无 | 创建新的同步配置文件。 |
| [删除同步配置文件](../api/educationsynchronizationprofile-delete.md) | **educationSynchronizationProfile** | 在给定配置文件标识符的情况删除特定配置文件。 |
| [暂停正在进行的同步](../api/educationsynchronizationprofile-pause.md) | 无 | 暂停正在进行的同步。 |
| [恢复暂停的同步](../api/educationsynchronizationprofile-resume.md) | 无 | 恢复暂停的同步。 |
| [重置同步](../api/educationsynchronizationprofile-reset.md) | 无 | 重置配置文件的状态并重新启动同步。 |
| [开始同步上载的文件](../api/educationsynchronizationprofile-start.md) | [educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)集合| 验证上载的源文件并启动同步。 仅在数据提供程序为[educationCsvDataProvider](educationcsvdataprovider.md)时适用。 |
| [获取上载 URL](../api/educationsynchronizationprofile-uploadurl.md) | string | 返回短生存期的 URL 以上载 CSV 数据文件。 仅在数据提供程序为[educationCsvDataProvider](educationcsvdataprovider.md)时适用。 |
| [获取同步状态](../api/educationsynchronizationprofilestatus-get.md) | [status](educationsynchronizationprofilestatus.md) | 返回特定同步配置文件的状态。 |
| [获取同步错误](../api/educationsynchronizationerrors-get.md) | [educationSynchronizationError](educationsynchronizationerror.md)集合| 获取同步过程中生成的所有错误。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **displayName** | string |  用于同步标识的配置文件的名称。         |
| **dataProvider** | [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md) |  用于配置文件的数据提供程序。         |
| **identitySynchronizationConfiguration** | [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md) | 标识的[创建](educationidentitycreationconfiguration.md)或[匹配](educationidentitymatchingconfiguration.md)配置。        |
| **licensesToAssign** | [educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)集合|  许可证安装程序配置。        |
| **state** | educationSynchronizationProfileState |  配置文件的状态。 可取值为：`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed`。          |

## <a name="relationships"></a>关系

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **errors** | [educationSynchronizationError](educationsynchronizationerror.md)集合| 与此同步配置文件关联的所有错误。 |
| **profileStatus** | [educationSynchronizationProfileStatus](educationsynchronizationprofilestatus.md) | 同步状态。 |

## <a name="json-representation"></a>JSON 表示形式
下面是**educationSynchronizationProfile**资源的 JSON 表示形式。

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
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```

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