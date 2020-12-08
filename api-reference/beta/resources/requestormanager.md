---
title: requestorManager 复杂类型
description: 标识将允许作为审批者的租户中另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca8559d3ecf7ba4110a7e2871f8e6acf545d2906
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581150"
---
# <a name="requestormanager-complex-type"></a><span data-ttu-id="9cb77-103">requestorManager 复杂类型</span><span class="sxs-lookup"><span data-stu-id="9cb77-103">requestorManager complex type</span></span>

<span data-ttu-id="9cb77-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cb77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cb77-105">在 [访问包分配策略](accesspackageassignmentpolicy.md)的审批设置中使用。</span><span class="sxs-lookup"><span data-stu-id="9cb77-105">Used in the approval settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="9cb77-106">它是 [userSet](userset.md)的子类型，其中 `@odata.type` 值 `#microsoft.graph.requestorManager` 表示请求用户的经理是审批者。</span><span class="sxs-lookup"><span data-stu-id="9cb77-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.requestorManager` indicates that a requesting user's manager is to be the approver.</span></span>  <span data-ttu-id="9cb77-107">在使用 requestorManager 创建访问包分配策略审批阶段时，还应包括另一个审批者（如单个用户或组成员），以防请求用户没有经理。</span><span class="sxs-lookup"><span data-stu-id="9cb77-107">When creating an access package assignment policy approval stage with requestorManager, also include another approver, such as a single user or group member, in case the requesting user does not have a manager.</span></span>


## <a name="properties"></a><span data-ttu-id="9cb77-108">属性</span><span class="sxs-lookup"><span data-stu-id="9cb77-108">Properties</span></span>


| <span data-ttu-id="9cb77-109">属性</span><span class="sxs-lookup"><span data-stu-id="9cb77-109">Property</span></span>                     | <span data-ttu-id="9cb77-110">类型</span><span class="sxs-lookup"><span data-stu-id="9cb77-110">Type</span></span>                      | <span data-ttu-id="9cb77-111">Description</span><span class="sxs-lookup"><span data-stu-id="9cb77-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="9cb77-112">isBackup</span><span class="sxs-lookup"><span data-stu-id="9cb77-112">isBackup</span></span> | <span data-ttu-id="9cb77-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="9cb77-113">Boolean</span></span> | <span data-ttu-id="9cb77-114">对于审批阶段中的经理，指示管理器是否为备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="9cb77-114">For a manager in an approval stage, indicates whether the manager is a backup fallback approver.</span></span> |
|<span data-ttu-id="9cb77-115">managerLevel</span><span class="sxs-lookup"><span data-stu-id="9cb77-115">managerLevel</span></span> | <span data-ttu-id="9cb77-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9cb77-116">Int32</span></span> | <span data-ttu-id="9cb77-117">经理相对于请求者的层次结构级别。</span><span class="sxs-lookup"><span data-stu-id="9cb77-117">The hierarchical level of the manager with respect to the requestor.</span></span> <span data-ttu-id="9cb77-118">例如，请求者的直接经理的 managerLevel 为1，而请求者的经理的经理的 managerLevel 为2。</span><span class="sxs-lookup"><span data-stu-id="9cb77-118">For example, the direct manager of a requestor would have a managerLevel of 1, while the manager of the requestor's manager would have a managerLevel of 2.</span></span> <span data-ttu-id="9cb77-119">ManagerLevel 的默认值为1。</span><span class="sxs-lookup"><span data-stu-id="9cb77-119">Default value for managerLevel is 1.</span></span> <span data-ttu-id="9cb77-120">此属性的可能值范围为1到2。</span><span class="sxs-lookup"><span data-stu-id="9cb77-120">Possible values for this property range from 1 to 2.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9cb77-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9cb77-121">JSON representation</span></span>

<span data-ttu-id="9cb77-122">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cb77-122">The following is a JSON representation of the type.</span></span>

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


