---
title: identityProtectionRoot 资源类型
description: Microsoft 导航属性容器Graph标识保护资源。
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1d1ea31820743a0c132ee5f179b0917900a32e1a
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161983"
---
# <a name="identityprotectionroot-resource-type"></a>identityProtectionRoot 资源类型

命名空间：microsoft.graph

Microsoft 导航属性的容器Graph标识保护资源。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|riskDetections|[riskDetection](../resources/riskdetection.md) 集合| Identity Protection Azure AD中的风险检测，以及有关检测的关联信息。|
|riskyUsers|[riskyUser](../resources/riskyuser.md) 集合|Identity Protection 标记为处于风险Azure AD用户。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityProtectionRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityProtectionRoot"
}
```

