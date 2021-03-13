---
title: requestorManager 复杂类型
description: 标识与租户中将允许其成为审批者的另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b4bfd42854a55ec2daa9e380c539a25479b0e933
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761077"
---
# <a name="requestormanager-complex-type"></a><span data-ttu-id="c9ad3-103">requestorManager 复杂类型</span><span class="sxs-lookup"><span data-stu-id="c9ad3-103">requestorManager complex type</span></span>

<span data-ttu-id="c9ad3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9ad3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9ad3-105">在访问包分配策略的 [审批设置中使用](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="c9ad3-105">Used in the approval settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="c9ad3-106">它是 [userSet](userset.md)的子类型，其中值指示请求用户的经理 `@odata.type` `#microsoft.graph.requestorManager` 是审批者。</span><span class="sxs-lookup"><span data-stu-id="c9ad3-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.requestorManager` indicates that a requesting user's manager is to be the approver.</span></span>  <span data-ttu-id="c9ad3-107">使用 requestorManager 创建访问包分配策略审批阶段时，还应包括另一个审批者，如单个用户或组的成员，以防请求的用户没有经理。</span><span class="sxs-lookup"><span data-stu-id="c9ad3-107">When creating an access package assignment policy approval stage with requestorManager, also include another approver, such as a single user or group member, in case the requesting user does not have a manager.</span></span>


## <a name="properties"></a><span data-ttu-id="c9ad3-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9ad3-108">Properties</span></span>


| <span data-ttu-id="c9ad3-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9ad3-109">Property</span></span>                     | <span data-ttu-id="c9ad3-110">类型</span><span class="sxs-lookup"><span data-stu-id="c9ad3-110">Type</span></span>                      | <span data-ttu-id="c9ad3-111">说明</span><span class="sxs-lookup"><span data-stu-id="c9ad3-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="c9ad3-112">isBackup</span><span class="sxs-lookup"><span data-stu-id="c9ad3-112">isBackup</span></span> | <span data-ttu-id="c9ad3-113">布尔</span><span class="sxs-lookup"><span data-stu-id="c9ad3-113">Boolean</span></span> | <span data-ttu-id="c9ad3-114">对于处于审批阶段的经理，指示该经理是否是备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="c9ad3-114">For a manager in an approval stage, indicates whether the manager is a backup fallback approver.</span></span> |
|<span data-ttu-id="c9ad3-115">managerLevel</span><span class="sxs-lookup"><span data-stu-id="c9ad3-115">managerLevel</span></span> | <span data-ttu-id="c9ad3-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c9ad3-116">Int32</span></span> | <span data-ttu-id="c9ad3-117">请求者与经理的层次结构级别。</span><span class="sxs-lookup"><span data-stu-id="c9ad3-117">The hierarchical level of the manager with respect to the requestor.</span></span> <span data-ttu-id="c9ad3-118">例如，请求者的直接经理的 managerLevel 为 1，而请求者经理的经理的 managerLevel 为 2。</span><span class="sxs-lookup"><span data-stu-id="c9ad3-118">For example, the direct manager of a requestor would have a managerLevel of 1, while the manager of the requestor's manager would have a managerLevel of 2.</span></span> <span data-ttu-id="c9ad3-119">managerLevel 的默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="c9ad3-119">Default value for managerLevel is 1.</span></span> <span data-ttu-id="c9ad3-120">此属性的可能值范围为 1 到 2。</span><span class="sxs-lookup"><span data-stu-id="c9ad3-120">Possible values for this property range from 1 to 2.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c9ad3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9ad3-121">JSON representation</span></span>

<span data-ttu-id="c9ad3-122">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9ad3-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "managerLevel": 1
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


