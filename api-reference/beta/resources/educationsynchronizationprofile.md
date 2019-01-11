---
title: educationSynchronizationProfile 资源类型
description: 代表一组配置用于同步教育实体和 Azure Active Directory (Azure AD) 从源目录名单信息。 此资源提供了用于学校数据同步的编程表示。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 7ed8cf39ff8ccd2b8cb4c5b5e31350fec6202d01
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882920"
---
# <a name="educationsynchronizationprofile-resource-type"></a>educationSynchronizationProfile 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表一组配置用于同步教育实体和 Azure Active Directory (Azure AD) 从源目录名单信息。 此资源提供了用于[学校数据同步](https://sds.microsoft.com)的编程表示。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-|:-|:-|
| [列表同步配置文件](../api/educationsynchronizationprofile-list.md) | **educationSynchronizationProfile**集合 | 获取为租户中的所有同步配置文件的列表。 |
| [获取同步配置文件](../api/educationsynchronizationprofile-get.md) | **educationSynchronizationProfile** | 检索给定的配置文件标识符特定配置文件。 |
| [创建同步配置文件](../api/educationsynchronizationprofile-post.md) | 无 | 创建一个新的同步配置文件。 |
| [删除同步配置文件](../api/educationsynchronizationprofile-delete.md) | **educationSynchronizationProfile** | 删除特定的配置文件给定的配置文件标识符。 |
| [暂停正在进行同步](../api/educationsynchronizationprofile-pause.md) | 无 | 暂停正在进行的同步。 |
| [恢复暂停的同步](../api/educationsynchronizationprofile-resume.md) | 无 | 恢复暂停的同步。 |
| [重置 sync](../api/educationsynchronizationprofile-reset.md) | 无 | 重置配置文件的状态，并重新启动同步。 |
| [启动同步上载文件](../api/educationsynchronizationprofile-start.md) | [educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)集合| 验证已上载的源文件，并启动同步。 应用仅数据提供程序何时[educationCsvDataProvider](educationcsvdataprovider.md)。 |
| [获取一个上载 URL](../api/educationsynchronizationprofile-uploadurl.md) | string | 返回要上载 CSV 数据文件的短期 URL。 应用仅数据提供程序何时[educationCsvDataProvider](educationcsvdataprovider.md)。 |
| [要获取同步的状态](../api/educationsynchronizationprofilestatus-get.md) | [status](educationsynchronizationprofilestatus.md) | 返回一个特定的同步配置文件的状态。 |
| [获取同步错误](../api/educationsynchronizationerrors-get.md) | [educationSynchronizationError](educationsynchronizationerror.md)集合| 获取所有同步过程中生成的错误。 |

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:-|:-|:-|
| **displayName** | string |  配置文件的同步标识名称。         |
| **dataProvider** | [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md) |  用于配置文件数据提供程序。         |
| **identitysynchronizationconfiguration** | [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md) | 标识[创建](educationidentitycreationconfiguration.md)或[匹配](educationidentitymatchingconfiguration.md)配置。        |
| **licensesToAssign** | [educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)集合|  许可证安装配置。        |
| **state** | string |  配置文件的状态。 可取值为：`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed`。          |

## <a name="relationships"></a>Relationships

| 属性 | 类型 | Description |
|:-|:-|:-|
| **errors** | [educationSynchronizationError](educationsynchronizationerror.md)集合| 与此同步配置文件关联的所有错误。 |
| **profileStatus** | [educationSynchronizationProfileStatus](educationsynchronizationprofilestatus.md) | 同步状态。 |

## <a name="json-representation"></a>JSON 表示形式
下面是**educationSynchronizationProfile**资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
    "displayName": "String",
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "#microsoft.graph.educationcsvdataprovider" },
    "identitySynchronizationConfiguration": { "@odata.type": "#microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
