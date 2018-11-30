---
title: resourceReference 资源类型
description: 包含属性的见解复杂类型。
ms.openlocfilehash: d171151a1c3547aa6863a7f70cc3a42ddec13e5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046280"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="1c205-103">resourceReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c205-103">resourceReference resource type</span></span>

> <span data-ttu-id="1c205-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c205-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c205-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c205-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c205-106">包含属性的[见解](insights.md)复杂类型。</span><span class="sxs-lookup"><span data-stu-id="1c205-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c205-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c205-107">JSON representation</span></span>

<span data-ttu-id="1c205-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c205-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="1c205-109">属性</span><span class="sxs-lookup"><span data-stu-id="1c205-109">Properties</span></span>

| <span data-ttu-id="1c205-110">属性</span><span class="sxs-lookup"><span data-stu-id="1c205-110">Property</span></span>      | <span data-ttu-id="1c205-111">类型</span><span class="sxs-lookup"><span data-stu-id="1c205-111">Type</span></span>      | <span data-ttu-id="1c205-112">说明</span><span class="sxs-lookup"><span data-stu-id="1c205-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="1c205-113">WebUrl</span><span class="sxs-lookup"><span data-stu-id="1c205-113">webUrl</span></span>        | <span data-ttu-id="1c205-114">String</span><span class="sxs-lookup"><span data-stu-id="1c205-114">String</span></span>    | <span data-ttu-id="1c205-115">通向引用的项的 URL。</span><span class="sxs-lookup"><span data-stu-id="1c205-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="1c205-116">id</span><span class="sxs-lookup"><span data-stu-id="1c205-116">id</span></span>            | <span data-ttu-id="1c205-117">字符串</span><span class="sxs-lookup"><span data-stu-id="1c205-117">String</span></span>    | <span data-ttu-id="1c205-118">项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1c205-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="1c205-119">type</span><span class="sxs-lookup"><span data-stu-id="1c205-119">type</span></span>          | <span data-ttu-id="1c205-120">字符串</span><span class="sxs-lookup"><span data-stu-id="1c205-120">String</span></span>    | <span data-ttu-id="1c205-121">一个 string 值，可以用于分类项目，如"microsoft.graph.driveItem"</span><span class="sxs-lookup"><span data-stu-id="1c205-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |