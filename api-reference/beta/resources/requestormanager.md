---
title: requestorManager 复杂类型
description: 标识将允许作为审批者的租户中另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b7eea64e2d3f1d32b7ca60fc0c3a548401f7ef23
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331350"
---
# <a name="requestomanager-complex-type"></a><span data-ttu-id="fd835-103">requestoManager 复杂类型</span><span class="sxs-lookup"><span data-stu-id="fd835-103">requestoManager complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd835-104">在[访问包分配策略](accesspackageassignmentpolicy.md)的审批设置中使用。</span><span class="sxs-lookup"><span data-stu-id="fd835-104">Used in the approval settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="fd835-105">它是[userSet](userset.md)的子类型，其中`@odata.type`值`#microsoft.graph.requestorManager`表示请求用户的经理是审批者。</span><span class="sxs-lookup"><span data-stu-id="fd835-105">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.requestorManager` indicates that a requesting user's manager is to be the approver.</span></span>  <span data-ttu-id="fd835-106">在使用 requestorManager 创建访问包分配策略审批阶段时，还应包括另一个审批者（如单个用户或组成员），以防请求用户没有经理。</span><span class="sxs-lookup"><span data-stu-id="fd835-106">When creating an access package assignment policy approval stage with requestorManager, also include another approver, such as a single user or group member, in case the requesting user does not have a manager.</span></span>


## <a name="properties"></a><span data-ttu-id="fd835-107">属性</span><span class="sxs-lookup"><span data-stu-id="fd835-107">Properties</span></span>


| <span data-ttu-id="fd835-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd835-108">Property</span></span>                     | <span data-ttu-id="fd835-109">类型</span><span class="sxs-lookup"><span data-stu-id="fd835-109">Type</span></span>                      | <span data-ttu-id="fd835-110">说明</span><span class="sxs-lookup"><span data-stu-id="fd835-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="fd835-111">isBackup</span><span class="sxs-lookup"><span data-stu-id="fd835-111">isBackup</span></span> | <span data-ttu-id="fd835-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="fd835-112">Boolean</span></span> | <span data-ttu-id="fd835-113">对于审批阶段中的经理，指示管理器是否为备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="fd835-113">For a manager in an approval stage, indicates whether the manager is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fd835-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd835-114">JSON representation</span></span>

<span data-ttu-id="fd835-115">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd835-115">The following is a JSON representation of the type.</span></span>

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
