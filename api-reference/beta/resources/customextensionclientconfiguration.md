---
title: customExtensionClientConfiguration 资源类型
description: HTTP 连接设置，用于Azure AD逻辑应用在关闭连接之前等待响应。 仅支持 timeoutInMilliseconds。
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2c04e53560aecc3e41978b569e42d993477eca87
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338408"
---
# <a name="customextensionclientconfiguration-resource-type"></a>customExtensionClientConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

HTTP 连接设置，用于Azure AD逻辑应用在关闭连接之前等待响应。 仅 **支持 timeoutInMilliseconds** 。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|timeoutInMilliseconds|Int32|在关闭连接之前，Azure AD等待逻辑应用响应的最大持续时间（以毫秒为单位）。 有效范围介于和 `200` 毫秒 `2000` 之间。 默认持续时间为 `1000`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customExtensionClientConfiguration",
  "timeoutInMilliseconds": "Integer"
}
```

