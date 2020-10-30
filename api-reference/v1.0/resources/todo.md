---
title: todo 资源类型
description: 表示用户可以使用的微软待办服务。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: aa468c6d6556ad70d3650e40fb3fd01c46ccdb35
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797286"
---
# <a name="todo-resource-type"></a><span data-ttu-id="a28dc-103">todo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a28dc-103">todo resource type</span></span>

<span data-ttu-id="a28dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a28dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a28dc-105">表示用户可以使用的微软待办服务。</span><span class="sxs-lookup"><span data-stu-id="a28dc-105">Represents the To Do services available to a user.</span></span>

<span data-ttu-id="a28dc-106">继承自 [entity](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="a28dc-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a28dc-107">方法</span><span class="sxs-lookup"><span data-stu-id="a28dc-107">Methods</span></span>
|<span data-ttu-id="a28dc-108">方法</span><span class="sxs-lookup"><span data-stu-id="a28dc-108">Method</span></span>|<span data-ttu-id="a28dc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a28dc-109">Return type</span></span>|<span data-ttu-id="a28dc-110">说明</span><span class="sxs-lookup"><span data-stu-id="a28dc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a28dc-111">列出列表</span><span class="sxs-lookup"><span data-stu-id="a28dc-111">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="a28dc-112">[todoTaskList](todotasklist.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a28dc-112">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="a28dc-113">获取用户邮箱中的所有任务列表。</span><span class="sxs-lookup"><span data-stu-id="a28dc-113">Get all the task lists in the user's mailbox.</span></span> |
|[<span data-ttu-id="a28dc-114">创建 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="a28dc-114">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="a28dc-115">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="a28dc-115">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="a28dc-116">在用户的邮箱中创建微软待办任务列表。</span><span class="sxs-lookup"><span data-stu-id="a28dc-116">Create a To Do task list in the user's mailbox.</span></span> |

## <a name="properties"></a><span data-ttu-id="a28dc-117">属性</span><span class="sxs-lookup"><span data-stu-id="a28dc-117">Properties</span></span>
<span data-ttu-id="a28dc-118">无</span><span class="sxs-lookup"><span data-stu-id="a28dc-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a28dc-119">关系</span><span class="sxs-lookup"><span data-stu-id="a28dc-119">Relationships</span></span>
|<span data-ttu-id="a28dc-120">关系</span><span class="sxs-lookup"><span data-stu-id="a28dc-120">Relationship</span></span>|<span data-ttu-id="a28dc-121">类型</span><span class="sxs-lookup"><span data-stu-id="a28dc-121">Type</span></span>|<span data-ttu-id="a28dc-122">说明</span><span class="sxs-lookup"><span data-stu-id="a28dc-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a28dc-123">lists</span><span class="sxs-lookup"><span data-stu-id="a28dc-123">lists</span></span>|<span data-ttu-id="a28dc-124">[todoTaskList](../resources/todotasklist.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a28dc-124">[todoTaskList](../resources/todotasklist.md) collection</span></span>| <span data-ttu-id="a28dc-125">"用户" 邮箱中的任务列表。</span><span class="sxs-lookup"><span data-stu-id="a28dc-125">The task lists in the users mailbox.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a28dc-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a28dc-126">JSON representation</span></span>
<span data-ttu-id="a28dc-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a28dc-127">The following is a JSON representation of the resource.</span></span>
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



