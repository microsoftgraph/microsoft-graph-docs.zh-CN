---
title: securityActionState 资源类型
description: 表示 securityAction 状态更改的历史记录。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6a2fecbc05c9987ee8daec8fa017d728a2d03ed3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722088"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="1c65b-103">securityActionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c65b-103">securityActionState resource type</span></span>

<span data-ttu-id="1c65b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c65b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c65b-105">表示 securityAction 状态更改的历史记录。</span><span class="sxs-lookup"><span data-stu-id="1c65b-105">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="1c65b-106">属性</span><span class="sxs-lookup"><span data-stu-id="1c65b-106">Properties</span></span>

| <span data-ttu-id="1c65b-107">属性</span><span class="sxs-lookup"><span data-stu-id="1c65b-107">Property</span></span>     | <span data-ttu-id="1c65b-108">类型</span><span class="sxs-lookup"><span data-stu-id="1c65b-108">Type</span></span>        | <span data-ttu-id="1c65b-109">说明</span><span class="sxs-lookup"><span data-stu-id="1c65b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c65b-110">appId</span><span class="sxs-lookup"><span data-stu-id="1c65b-110">appId</span></span>|<span data-ttu-id="1c65b-111">String</span><span class="sxs-lookup"><span data-stu-id="1c65b-111">String</span></span>|<span data-ttu-id="1c65b-112">提交更新的调用应用程序的应用程序 ID (PATCH) 操作。</span><span class="sxs-lookup"><span data-stu-id="1c65b-112">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="1c65b-113">应 `appId` 从身份验证令牌中提取，调用应用程序不应手动输入。</span><span class="sxs-lookup"><span data-stu-id="1c65b-113">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="1c65b-114">状态</span><span class="sxs-lookup"><span data-stu-id="1c65b-114">status</span></span>|<span data-ttu-id="1c65b-115">String</span><span class="sxs-lookup"><span data-stu-id="1c65b-115">String</span></span>| <span data-ttu-id="1c65b-116">此更新中 securityAction 的状态。</span><span class="sxs-lookup"><span data-stu-id="1c65b-116">Status of the securityAction in this update.</span></span> <span data-ttu-id="1c65b-117">可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。</span><span class="sxs-lookup"><span data-stu-id="1c65b-117">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="1c65b-118">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c65b-118">updatedDateTime</span></span>|<span data-ttu-id="1c65b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c65b-119">DateTimeOffset</span></span>| <span data-ttu-id="1c65b-120">actionState 更新后的时间戳。</span><span class="sxs-lookup"><span data-stu-id="1c65b-120">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="1c65b-121">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1c65b-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1c65b-122">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1c65b-122">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1c65b-123">user</span><span class="sxs-lookup"><span data-stu-id="1c65b-123">user</span></span>|<span data-ttu-id="1c65b-124">String</span><span class="sxs-lookup"><span data-stu-id="1c65b-124">String</span></span>|<span data-ttu-id="1c65b-125">提交更新的登录用户的用户主体名称 (PATCH) 操作。</span><span class="sxs-lookup"><span data-stu-id="1c65b-125">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="1c65b-126">应 `user` 从身份验证令牌中提取，调用应用程序不应手动输入。</span><span class="sxs-lookup"><span data-stu-id="1c65b-126">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c65b-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c65b-127">JSON representation</span></span>

<span data-ttu-id="1c65b-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c65b-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


