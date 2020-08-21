---
title: todo 资源类型
description: 表示用户可用的 To Do 服务。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 99b2936cf84c5cfdc25a39ff6f0e35518658d0ff
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849872"
---
# <a name="todo-resource-type"></a><span data-ttu-id="e372b-103">todo 资源类型</span><span class="sxs-lookup"><span data-stu-id="e372b-103">todo resource type</span></span>

<span data-ttu-id="e372b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e372b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e372b-105">表示用户可用的 To Do 服务。</span><span class="sxs-lookup"><span data-stu-id="e372b-105">Represents the To Do services available to a user.</span></span>

<span data-ttu-id="e372b-106">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="e372b-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e372b-107">方法</span><span class="sxs-lookup"><span data-stu-id="e372b-107">Methods</span></span>
|<span data-ttu-id="e372b-108">方法</span><span class="sxs-lookup"><span data-stu-id="e372b-108">Method</span></span>|<span data-ttu-id="e372b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e372b-109">Return type</span></span>|<span data-ttu-id="e372b-110">说明</span><span class="sxs-lookup"><span data-stu-id="e372b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e372b-111">列表列表</span><span class="sxs-lookup"><span data-stu-id="e372b-111">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="e372b-112">[todoTaskList](todotasklist.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e372b-112">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="e372b-113">获取用户邮箱中的所有任务列表。</span><span class="sxs-lookup"><span data-stu-id="e372b-113">Get all the task lists in the user's mailbox.</span></span> |
|[<span data-ttu-id="e372b-114">创建 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="e372b-114">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="e372b-115">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="e372b-115">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="e372b-116">在用户邮箱中创建"执行"任务列表。</span><span class="sxs-lookup"><span data-stu-id="e372b-116">Create a To Do task list in the user's mailbox.</span></span> |

## <a name="properties"></a><span data-ttu-id="e372b-117">属性</span><span class="sxs-lookup"><span data-stu-id="e372b-117">Properties</span></span>
<span data-ttu-id="e372b-118">无</span><span class="sxs-lookup"><span data-stu-id="e372b-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e372b-119">关系</span><span class="sxs-lookup"><span data-stu-id="e372b-119">Relationships</span></span>
|<span data-ttu-id="e372b-120">关系</span><span class="sxs-lookup"><span data-stu-id="e372b-120">Relationship</span></span>|<span data-ttu-id="e372b-121">类型</span><span class="sxs-lookup"><span data-stu-id="e372b-121">Type</span></span>|<span data-ttu-id="e372b-122">说明</span><span class="sxs-lookup"><span data-stu-id="e372b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e372b-123">lists</span><span class="sxs-lookup"><span data-stu-id="e372b-123">lists</span></span>|<span data-ttu-id="e372b-124">[todoTaskList](../resources/todotasklist.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e372b-124">[todoTaskList](../resources/todotasklist.md) collection</span></span>| <span data-ttu-id="e372b-125">用户邮箱中的任务列表。</span><span class="sxs-lookup"><span data-stu-id="e372b-125">The task lists in the users mailbox.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e372b-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e372b-126">JSON representation</span></span>
<span data-ttu-id="e372b-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e372b-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todo",
  "id": "String"
}
```

