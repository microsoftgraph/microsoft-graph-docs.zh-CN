---
title: groupPolicyPresentationListBox 资源类型
description: 表示 ADMX listBox 元素和 ADMX 列表元素。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01eb53e7053fcc2209cafb70ac925b109fb340a1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046832"
---
# <a name="grouppolicypresentationlistbox-resource-type"></a>groupPolicyPresentationListBox 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 ADMX listBox 元素和 ADMX 列表元素。


继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyPresentationListBoxes](../api/intune-grouppolicy-grouppolicypresentationlistbox-list.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) 集合|列出 [groupPolicyPresentationListBox 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) 关系。|
|[获取 groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-get.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|读取 [groupPolicyPresentationListBox 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) 关系。|
|[创建 groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-create.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|创建新的 [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) 对象。|
|[删除 groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-delete.md)|无|删除 [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)。|
|[更新 groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-update.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|更新 [groupPolicyPresentationListBox 对象](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|标签|String|任何演示文稿实体的本地化文本标签。 默认值为空白。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|实体的键。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|explicitValue|Boolean|如果指定此选项，则用户必须指定注册表子项值和注册表子项名称。 列表框显示两列，一列用于名称，另一列用于数据。 默认值为 false。|
|valuePrefix|String|尚未记录|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|与演示文稿关联的组策略定义。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationListBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "explicitValue": true,
  "valuePrefix": "String"
}
```



