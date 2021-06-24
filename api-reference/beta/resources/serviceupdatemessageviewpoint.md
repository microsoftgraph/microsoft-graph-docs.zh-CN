---
title: serviceUpdateMessageViewpoint 资源类型
description: 表示 serviceUpdateMessage 的用户视图点数据。"
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c84a07691c2507a9ff74102ac6f4b1675cb382e7
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109092"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a><span data-ttu-id="4d001-103">serviceUpdateMessageViewpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d001-103">serviceUpdateMessageViewpoint resource type</span></span>

<span data-ttu-id="4d001-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d001-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d001-105">表示 [serviceUpdateMessage](../resources/serviceupdatemessage.md)的用户视图点数据。</span><span class="sxs-lookup"><span data-stu-id="4d001-105">Represents user view points data for a [serviceUpdateMessage](../resources/serviceupdatemessage.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4d001-106">属性</span><span class="sxs-lookup"><span data-stu-id="4d001-106">Properties</span></span>
|<span data-ttu-id="4d001-107">属性</span><span class="sxs-lookup"><span data-stu-id="4d001-107">Property</span></span>|<span data-ttu-id="4d001-108">类型</span><span class="sxs-lookup"><span data-stu-id="4d001-108">Type</span></span>|<span data-ttu-id="4d001-109">说明</span><span class="sxs-lookup"><span data-stu-id="4d001-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d001-110">isArchived</span><span class="sxs-lookup"><span data-stu-id="4d001-110">isArchived</span></span>|<span data-ttu-id="4d001-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d001-111">Boolean</span></span>|<span data-ttu-id="4d001-112">指示用户是否已存档邮件。</span><span class="sxs-lookup"><span data-stu-id="4d001-112">Indicates whether the user archived the message.</span></span>|
|<span data-ttu-id="4d001-113">isFavorited</span><span class="sxs-lookup"><span data-stu-id="4d001-113">isFavorited</span></span>|<span data-ttu-id="4d001-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="4d001-114">Boolean</span></span>|<span data-ttu-id="4d001-115">指示用户是否将邮件标记为收藏夹。</span><span class="sxs-lookup"><span data-stu-id="4d001-115">Indicates whether the user marked the message as favorite.</span></span>|
|<span data-ttu-id="4d001-116">isRead</span><span class="sxs-lookup"><span data-stu-id="4d001-116">isRead</span></span>|<span data-ttu-id="4d001-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d001-117">Boolean</span></span>|<span data-ttu-id="4d001-118">指示用户是否阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="4d001-118">Indicates whether the user read the message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d001-119">关系</span><span class="sxs-lookup"><span data-stu-id="4d001-119">Relationships</span></span>
<span data-ttu-id="4d001-120">无。</span><span class="sxs-lookup"><span data-stu-id="4d001-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d001-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d001-121">JSON representation</span></span>
<span data-ttu-id="4d001-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d001-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessageViewpoint",
  "isRead": "Boolean",
  "isArchived": "Boolean",
  "isFavorited": "Boolean"
}
```