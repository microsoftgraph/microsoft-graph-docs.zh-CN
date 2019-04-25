---
title: securityActionState 资源类型
description: 表示 securityAction 状态更改的历史记录。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8f789dab438316f16b9c2607947fa08b7fcefdc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522018"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="df7f2-103">securityActionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="df7f2-103">securityActionState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df7f2-104">表示 securityAction 状态更改的历史记录。</span><span class="sxs-lookup"><span data-stu-id="df7f2-104">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="df7f2-105">属性</span><span class="sxs-lookup"><span data-stu-id="df7f2-105">Properties</span></span>

| <span data-ttu-id="df7f2-106">属性</span><span class="sxs-lookup"><span data-stu-id="df7f2-106">Property</span></span>     | <span data-ttu-id="df7f2-107">类型</span><span class="sxs-lookup"><span data-stu-id="df7f2-107">Type</span></span>        | <span data-ttu-id="df7f2-108">说明</span><span class="sxs-lookup"><span data-stu-id="df7f2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df7f2-109">appId</span><span class="sxs-lookup"><span data-stu-id="df7f2-109">appId</span></span>|<span data-ttu-id="df7f2-110">String</span><span class="sxs-lookup"><span data-stu-id="df7f2-110">String</span></span>|<span data-ttu-id="df7f2-111">向操作提交更新 (修补程序) 的呼叫应用程序的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="df7f2-111">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="df7f2-112">`appId`应从 auth 令牌中提取, 而不是通过调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="df7f2-112">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="df7f2-113">状态</span><span class="sxs-lookup"><span data-stu-id="df7f2-113">status</span></span>|<span data-ttu-id="df7f2-114">字符串</span><span class="sxs-lookup"><span data-stu-id="df7f2-114">String</span></span>| <span data-ttu-id="df7f2-115">此更新中的 securityAction 的状态。</span><span class="sxs-lookup"><span data-stu-id="df7f2-115">Status of the securityAction in this update.</span></span> <span data-ttu-id="df7f2-116">可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。</span><span class="sxs-lookup"><span data-stu-id="df7f2-116">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="df7f2-117">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="df7f2-117">updatedDateTime</span></span>|<span data-ttu-id="df7f2-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df7f2-118">DateTimeOffset</span></span>| <span data-ttu-id="df7f2-119">更新 actionState 时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="df7f2-119">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="df7f2-120">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="df7f2-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="df7f2-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="df7f2-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="df7f2-122">user</span><span class="sxs-lookup"><span data-stu-id="df7f2-122">user</span></span>|<span data-ttu-id="df7f2-123">String</span><span class="sxs-lookup"><span data-stu-id="df7f2-123">String</span></span>|<span data-ttu-id="df7f2-124">向操作提交更新 (修补程序) 的已登录用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="df7f2-124">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="df7f2-125">`user`应从 auth 令牌中提取, 而不是通过调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="df7f2-125">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df7f2-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df7f2-126">JSON representation</span></span>

<span data-ttu-id="df7f2-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df7f2-127">The following is a JSON representation of the resource.</span></span>

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
