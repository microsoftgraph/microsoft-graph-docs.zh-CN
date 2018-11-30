---
title: recordingInfo 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 92af3fcb52ab08f3f25a2c16cc720a4053a9bdfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044796"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="4c618-103">recordingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c618-103">recordingInfo resource type</span></span>

> <span data-ttu-id="4c618-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4c618-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c618-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4c618-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="4c618-106">属性</span><span class="sxs-lookup"><span data-stu-id="4c618-106">Properties</span></span>

| <span data-ttu-id="4c618-107">属性</span><span class="sxs-lookup"><span data-stu-id="4c618-107">Property</span></span>       | <span data-ttu-id="4c618-108">类型</span><span class="sxs-lookup"><span data-stu-id="4c618-108">Type</span></span>    | <span data-ttu-id="4c618-109">说明</span><span class="sxs-lookup"><span data-stu-id="4c618-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c618-110">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="4c618-110">initiatedBy</span></span> | [<span data-ttu-id="4c618-111">participantInfo</span><span class="sxs-lookup"><span data-stu-id="4c618-111">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="4c618-112">参与者发起录制。</span><span class="sxs-lookup"><span data-stu-id="4c618-112">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="4c618-113">状态</span><span class="sxs-lookup"><span data-stu-id="4c618-113">status</span></span> | <span data-ttu-id="4c618-114">字符串</span><span class="sxs-lookup"><span data-stu-id="4c618-114">String</span></span> | <span data-ttu-id="4c618-115">可取值为：`recordingCapable`、`notRecording`、`startedRecording`。</span><span class="sxs-lookup"><span data-stu-id="4c618-115">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c618-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c618-116">JSON representation</span></span>

<span data-ttu-id="4c618-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c618-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "status": "recordingCapable | notRecording | startedRecording"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
