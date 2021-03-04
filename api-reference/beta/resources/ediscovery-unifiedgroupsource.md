---
title: unifiedGroupSource 资源类型
description: 保管人组容器。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b6d1b1d1a7d3abee2516e170fcead20c73235f1f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446651"
---
# <a name="unifiedgroupsource-resource-type"></a>unifiedGroupSource 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

保管人 [组的容器](ediscovery-custodian.md) 。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 集合|获取 **unifiedGroupSource** 对象及其属性的列表。|
|[创建 unifiedGroupSource](../api/ediscovery-custodian-post-unifiedgroupsources.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|创建新的 **unifiedGroupSource** 对象。|
|[获取 unifiedGroupSource](../api/ediscovery-unifiedgroupsource-get.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|读取 **unifiedGroupSource** 对象的属性和关系。|
|[删除 unifiedGroupSource](../api/ediscovery-unifiedgroupsource-delete.md)|无|删除 **unifiedGroupSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **unifiedGroupSource 的用户**。|
|createdDateTime|DateTimeOffset|创建 **unifiedGroupSource 的** 日期和时间。|
|displayName|String|统显示名称的名称 - 这是组的名称。|
|id|String|**unifiedGroupSource** 的 ID。 这不是实际组的 ID。|
|includedSources|microsoft.graph.ediscovery.sourceType|指定此组中包含的源。 可取值为：`mailbox`、`site`。|

### <a name="sourcetype-values"></a>sourceType 值

与用户相关的源类型。 默认情况下包括邮箱和网站。

|成员|说明|
|:----|-----------|
|邮箱|表示邮箱。|
|网站|表示 SharePoint 网站。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|group|[组](../resources/group.md)|与 **unifiedGroupSource** 关联的组。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.unifiedGroupSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
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
