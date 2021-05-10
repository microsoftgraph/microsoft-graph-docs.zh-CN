---
title: ticketInfo 资源类型
description: 表示与请求相关的票证角色分配的对象
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 584600bf017a75efb141539b6f1397920717fb76
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299209"
---
# <a name="ticketinfo-resource-type"></a><span data-ttu-id="774a8-103">ticketInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="774a8-103">ticketInfo resource type</span></span>

<span data-ttu-id="774a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="774a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="774a8-105">表示与请求相关的票证角色分配的对象</span><span class="sxs-lookup"><span data-stu-id="774a8-105">The object that represents ticket information related to role assignment requests</span></span>

## <a name="properties"></a><span data-ttu-id="774a8-106">属性</span><span class="sxs-lookup"><span data-stu-id="774a8-106">Properties</span></span>
|<span data-ttu-id="774a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="774a8-107">Property</span></span>|<span data-ttu-id="774a8-108">类型</span><span class="sxs-lookup"><span data-stu-id="774a8-108">Type</span></span>|<span data-ttu-id="774a8-109">说明</span><span class="sxs-lookup"><span data-stu-id="774a8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="774a8-110">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="774a8-110">ticketNumber</span></span>|<span data-ttu-id="774a8-111">String</span><span class="sxs-lookup"><span data-stu-id="774a8-111">String</span></span>|<span data-ttu-id="774a8-112">票证编号元数据</span><span class="sxs-lookup"><span data-stu-id="774a8-112">Ticket number meta data</span></span>|
|<span data-ttu-id="774a8-113">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="774a8-113">ticketSystem</span></span>|<span data-ttu-id="774a8-114">String</span><span class="sxs-lookup"><span data-stu-id="774a8-114">String</span></span>|<span data-ttu-id="774a8-115">票证系统元数据</span><span class="sxs-lookup"><span data-stu-id="774a8-115">Ticket system meta data</span></span>|

## <a name="relationships"></a><span data-ttu-id="774a8-116">关系</span><span class="sxs-lookup"><span data-stu-id="774a8-116">Relationships</span></span>
<span data-ttu-id="774a8-117">无。</span><span class="sxs-lookup"><span data-stu-id="774a8-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="774a8-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="774a8-118">JSON representation</span></span>
<span data-ttu-id="774a8-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="774a8-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ticketInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ticketInfo",
  "ticketNumber": "String",
  "ticketSystem": "String"
}
```

