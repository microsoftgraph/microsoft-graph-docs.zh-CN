---
title: unifiedGroupSource 资源类型
description: 管理员组的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 5fba2a994cda61f111739d98ea3a210c76ffeb23
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597589"
---
# <a name="unifiedgroupsource-resource-type"></a>unifiedGroupSource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[管理员](custodian.md)组的容器。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[列出 unifiedGroupSources](../api/custodian-list-unifiedgroupsources.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md) 集合|获取 **unifiedGroupSource** 对象及其属性的列表。|
|[创建 unifiedGroupSource](../api/custodian-post-unifiedgroupsources.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md)|创建新的 **unifiedGroupSource** 对象。|
|[获取 unifiedGroupSource](../api/unifiedgroupsource-get.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md)|读取 **unifiedGroupSource** 对象的属性和关系。|
|[删除 unifiedGroupSource](../api/unifiedgroupsource-delete.md)|无|删除 **unifiedGroupSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **unifiedGroupSource** 的用户。|
|createdDateTime|DateTimeOffset|**UnifiedGroupSource** 的创建日期和时间。|
|displayName|String|统一组的显示名称-这是组的名称。|
|id|String|**UnifiedGroupSource** 的 ID。 这不是实际组的 ID。|
|includedSources|sourceType|指定要包含在此组中的源。 可取值为：`mailbox`、`site`。|

### <a name="sourcetype-values"></a>sourceType 值

与用户相关的源的类型。 默认情况下包括邮箱和网站。

|成员|说明|
|:----|-----------|
|邮箱|代表一个邮箱。|
|网站|表示 SharePoint 网站。|

## <a name="relationships"></a>关系

|关系|类型|Description|
|:---|:---|:---|
|group|[组](../resources/group.md)|与 **unifiedGroupSource** 相关联的组。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedGroupSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "value": [
        {
            "displayName": "Developers group",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "33434233-3030-3739-3043-393039324633",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
