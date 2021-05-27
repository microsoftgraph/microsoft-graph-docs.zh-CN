---
title: ticketInfo 资源类型
description: 表示与请求相关的票证角色分配的对象
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a59b62ddb014dedd802af6fcde001d4791d729c3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682598"
---
# <a name="ticketinfo-resource-type"></a><span data-ttu-id="ffc9c-103">ticketInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffc9c-103">ticketInfo resource type</span></span>

<span data-ttu-id="ffc9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffc9c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffc9c-105">表示与请求相关的票证角色分配的对象</span><span class="sxs-lookup"><span data-stu-id="ffc9c-105">The object that represents ticket information related to role assignment requests</span></span>

## <a name="properties"></a><span data-ttu-id="ffc9c-106">属性</span><span class="sxs-lookup"><span data-stu-id="ffc9c-106">Properties</span></span>
|<span data-ttu-id="ffc9c-107">属性</span><span class="sxs-lookup"><span data-stu-id="ffc9c-107">Property</span></span>|<span data-ttu-id="ffc9c-108">类型</span><span class="sxs-lookup"><span data-stu-id="ffc9c-108">Type</span></span>|<span data-ttu-id="ffc9c-109">说明</span><span class="sxs-lookup"><span data-stu-id="ffc9c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffc9c-110">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="ffc9c-110">ticketNumber</span></span>|<span data-ttu-id="ffc9c-111">String</span><span class="sxs-lookup"><span data-stu-id="ffc9c-111">String</span></span>|<span data-ttu-id="ffc9c-112">票证编号元数据</span><span class="sxs-lookup"><span data-stu-id="ffc9c-112">Ticket number meta data</span></span>|
|<span data-ttu-id="ffc9c-113">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="ffc9c-113">ticketSystem</span></span>|<span data-ttu-id="ffc9c-114">String</span><span class="sxs-lookup"><span data-stu-id="ffc9c-114">String</span></span>|<span data-ttu-id="ffc9c-115">票证系统元数据</span><span class="sxs-lookup"><span data-stu-id="ffc9c-115">Ticket system meta data</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffc9c-116">关系</span><span class="sxs-lookup"><span data-stu-id="ffc9c-116">Relationships</span></span>
<span data-ttu-id="ffc9c-117">无。</span><span class="sxs-lookup"><span data-stu-id="ffc9c-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffc9c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffc9c-118">JSON representation</span></span>
<span data-ttu-id="ffc9c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffc9c-119">The following is a JSON representation of the resource.</span></span>
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

