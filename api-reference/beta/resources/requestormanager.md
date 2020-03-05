---
title: requestorManager 复杂类型
description: 标识将允许作为审批者的租户中另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b2e3062383dd1cc1c7d04342b2dcbd5be0afd67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521122"
---
# <a name="requestomanager-complex-type"></a><span data-ttu-id="dac8b-103">requestoManager 复杂类型</span><span class="sxs-lookup"><span data-stu-id="dac8b-103">requestoManager complex type</span></span>

<span data-ttu-id="dac8b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dac8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dac8b-105">在[访问包分配策略](accesspackageassignmentpolicy.md)的审批设置中使用。</span><span class="sxs-lookup"><span data-stu-id="dac8b-105">Used in the approval settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="dac8b-106">它是[userSet](userset.md)的子类型，其中`@odata.type`值`#microsoft.graph.requestorManager`表示请求用户的经理是审批者。</span><span class="sxs-lookup"><span data-stu-id="dac8b-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.requestorManager` indicates that a requesting user's manager is to be the approver.</span></span>  <span data-ttu-id="dac8b-107">在使用 requestorManager 创建访问包分配策略审批阶段时，还应包括另一个审批者（如单个用户或组成员），以防请求用户没有经理。</span><span class="sxs-lookup"><span data-stu-id="dac8b-107">When creating an access package assignment policy approval stage with requestorManager, also include another approver, such as a single user or group member, in case the requesting user does not have a manager.</span></span>


## <a name="properties"></a><span data-ttu-id="dac8b-108">属性</span><span class="sxs-lookup"><span data-stu-id="dac8b-108">Properties</span></span>


| <span data-ttu-id="dac8b-109">属性</span><span class="sxs-lookup"><span data-stu-id="dac8b-109">Property</span></span>                     | <span data-ttu-id="dac8b-110">类型</span><span class="sxs-lookup"><span data-stu-id="dac8b-110">Type</span></span>                      | <span data-ttu-id="dac8b-111">说明</span><span class="sxs-lookup"><span data-stu-id="dac8b-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="dac8b-112">isBackup</span><span class="sxs-lookup"><span data-stu-id="dac8b-112">isBackup</span></span> | <span data-ttu-id="dac8b-113">布尔</span><span class="sxs-lookup"><span data-stu-id="dac8b-113">Boolean</span></span> | <span data-ttu-id="dac8b-114">对于审批阶段中的经理，指示管理器是否为备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="dac8b-114">For a manager in an approval stage, indicates whether the manager is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dac8b-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dac8b-115">JSON representation</span></span>

<span data-ttu-id="dac8b-116">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dac8b-116">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorManager complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
