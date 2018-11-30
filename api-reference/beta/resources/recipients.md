---
title: 收件人资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: aa620fa920b4f91b2b2214f02c2e75d7a8cbcc4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048200"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="b74ee-103">收件人资源类型</span><span class="sxs-lookup"><span data-stu-id="b74ee-103">recipients resource type</span></span>

> <span data-ttu-id="b74ee-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b74ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b74ee-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b74ee-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b74ee-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b74ee-106">JSON representation</span></span>

<span data-ttu-id="b74ee-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b74ee-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipients"
}-->

```json
{
  "alias": "string",
  "email": "string",
  "objectId": "string",
  "permissionIdentityType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b74ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="b74ee-108">Properties</span></span>
| <span data-ttu-id="b74ee-109">属性</span><span class="sxs-lookup"><span data-stu-id="b74ee-109">Property</span></span>     | <span data-ttu-id="b74ee-110">类型</span><span class="sxs-lookup"><span data-stu-id="b74ee-110">Type</span></span>   |<span data-ttu-id="b74ee-111">说明</span><span class="sxs-lookup"><span data-stu-id="b74ee-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b74ee-112">alias</span><span class="sxs-lookup"><span data-stu-id="b74ee-112">alias</span></span>|<span data-ttu-id="b74ee-113">String</span><span class="sxs-lookup"><span data-stu-id="b74ee-113">String</span></span>||
|<span data-ttu-id="b74ee-114">email</span><span class="sxs-lookup"><span data-stu-id="b74ee-114">email</span></span>|<span data-ttu-id="b74ee-115">字符串</span><span class="sxs-lookup"><span data-stu-id="b74ee-115">String</span></span>||
|<span data-ttu-id="b74ee-116">objectId</span><span class="sxs-lookup"><span data-stu-id="b74ee-116">objectId</span></span>|<span data-ttu-id="b74ee-117">String</span><span class="sxs-lookup"><span data-stu-id="b74ee-117">String</span></span>||
|<span data-ttu-id="b74ee-118">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="b74ee-118">permissionIdentityType</span></span>|<span data-ttu-id="b74ee-119">String</span><span class="sxs-lookup"><span data-stu-id="b74ee-119">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->