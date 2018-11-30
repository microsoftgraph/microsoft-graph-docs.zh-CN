---
title: insightIdentity
description: " 资源类型"
ms.openlocfilehash: e13d08eb111844896c96b02ab22c52d2f598ce58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046081"
---
# <a name="insightidentity"></a><span data-ttu-id="9a49f-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="9a49f-103">insightIdentity</span></span>

> <span data-ttu-id="9a49f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9a49f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a49f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9a49f-105">Use of these APIs in production applications is not supported.</span></span>

 <span data-ttu-id="9a49f-106">资源类型</span><span class="sxs-lookup"><span data-stu-id="9a49f-106">resource type</span></span>

<span data-ttu-id="9a49f-107">包含[共享](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="9a49f-107">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="9a49f-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a49f-108">JSON representation</span></span>
<span data-ttu-id="9a49f-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a49f-109">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="9a49f-110">属性</span><span class="sxs-lookup"><span data-stu-id="9a49f-110">Properties</span></span>

| <span data-ttu-id="9a49f-111">属性</span><span class="sxs-lookup"><span data-stu-id="9a49f-111">Property</span></span>              | <span data-ttu-id="9a49f-112">类型</span><span class="sxs-lookup"><span data-stu-id="9a49f-112">Type</span></span>          | <span data-ttu-id="9a49f-113">说明</span><span class="sxs-lookup"><span data-stu-id="9a49f-113">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="9a49f-114">displayName</span><span class="sxs-lookup"><span data-stu-id="9a49f-114">displayName</span></span>       | <span data-ttu-id="9a49f-115">字符串</span><span class="sxs-lookup"><span data-stu-id="9a49f-115">String</span></span>          | <span data-ttu-id="9a49f-116">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9a49f-116">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="9a49f-117">id</span><span class="sxs-lookup"><span data-stu-id="9a49f-117">id</span></span>              | <span data-ttu-id="9a49f-118">字符串</span><span class="sxs-lookup"><span data-stu-id="9a49f-118">String</span></span>        | <span data-ttu-id="9a49f-119">共享项目的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="9a49f-119">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="9a49f-120">address</span><span class="sxs-lookup"><span data-stu-id="9a49f-120">address</span></span>             | <span data-ttu-id="9a49f-121">String</span><span class="sxs-lookup"><span data-stu-id="9a49f-121">String</span></span>      | <span data-ttu-id="9a49f-122">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9a49f-122">The email address of the user who shared the item.</span></span>  |