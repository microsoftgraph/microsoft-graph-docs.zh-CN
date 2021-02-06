---
title: accessPackageAnswerString 资源类型
description: accessPackageTextInputQuestion 的字符串答案
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: def7753e62239e403821ed6472b3613d025942ac
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132391"
---
# <a name="accesspackageanswerstring-resource-type"></a>accessPackageAnswerString 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示对 [accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md)的字符串输入答案。 存储在 [accessPackageAssignmentRequest 上](../resources/accesspackageassignmentrequest.md)。

继承自 [accessPackageAnswer](../resources/accesspackageanswer.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|答案适用的问题。 继承自 [accessPackageAnswer](../resources/accesspackageanswer.md)。|
|displayValue|字符串|向请求者和审批者显示的本地化显示值。 继承自 [accessPackageAnswer](../resources/accesspackageanswer.md)。|
|value|String|如果此答案配置为存储为特定属性，则存储在请求者用户配置文件上的值。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerString",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  },
  "value": "String"
}
```

