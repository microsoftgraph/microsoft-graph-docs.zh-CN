---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误
author: Jewan-microsoft
ms.openlocfilehash: 4cba6de22f08e2e41f281863e3494fbb589e6e41
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354780"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="11944-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="11944-103">onenoteOperationError resource type</span></span>

> <span data-ttu-id="11944-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="11944-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11944-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="11944-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11944-106">失败的 OneNote 操作中的错误</span><span class="sxs-lookup"><span data-stu-id="11944-106">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11944-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11944-107">JSON representation</span></span>

<span data-ttu-id="11944-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11944-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="11944-109">属性</span><span class="sxs-lookup"><span data-stu-id="11944-109">Properties</span></span>
| <span data-ttu-id="11944-110">属性</span><span class="sxs-lookup"><span data-stu-id="11944-110">Property</span></span>     | <span data-ttu-id="11944-111">类型</span><span class="sxs-lookup"><span data-stu-id="11944-111">Type</span></span>   |<span data-ttu-id="11944-112">说明</span><span class="sxs-lookup"><span data-stu-id="11944-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11944-113">code</span><span class="sxs-lookup"><span data-stu-id="11944-113">code</span></span>|<span data-ttu-id="11944-114">string</span><span class="sxs-lookup"><span data-stu-id="11944-114">string</span></span>|<span data-ttu-id="11944-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="11944-115">The error code.</span></span>|
|<span data-ttu-id="11944-116">消息</span><span class="sxs-lookup"><span data-stu-id="11944-116">message</span></span>|<span data-ttu-id="11944-117">string</span><span class="sxs-lookup"><span data-stu-id="11944-117">string</span></span>|<span data-ttu-id="11944-118">错误消息。</span><span class="sxs-lookup"><span data-stu-id="11944-118">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
