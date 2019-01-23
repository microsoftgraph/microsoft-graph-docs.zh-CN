---
title: iPv4Range 资源类型
description: 介绍 Intune，支持多个工作流的 Microsoft Graph api iPv4Range 资源。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9ac2656b7c79cceba70879fe478aec65a5bd7250
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425223"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="68648-103">iPv4Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="68648-103">iPv4Range resource type</span></span>

> <span data-ttu-id="68648-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="68648-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68648-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="68648-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68648-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="68648-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68648-107">IP V4 范围</span><span class="sxs-lookup"><span data-stu-id="68648-107">IP V4 range</span></span>

<span data-ttu-id="68648-108">继承自 [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="68648-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68648-109">属性</span><span class="sxs-lookup"><span data-stu-id="68648-109">Properties</span></span>
|<span data-ttu-id="68648-110">属性</span><span class="sxs-lookup"><span data-stu-id="68648-110">Property</span></span>|<span data-ttu-id="68648-111">类型</span><span class="sxs-lookup"><span data-stu-id="68648-111">Type</span></span>|<span data-ttu-id="68648-112">说明</span><span class="sxs-lookup"><span data-stu-id="68648-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68648-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="68648-113">lowerAddress</span></span>|<span data-ttu-id="68648-114">String</span><span class="sxs-lookup"><span data-stu-id="68648-114">String</span></span>|<span data-ttu-id="68648-115">IP 地址下限</span><span class="sxs-lookup"><span data-stu-id="68648-115">Lower IP Address</span></span>|
|<span data-ttu-id="68648-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="68648-116">upperAddress</span></span>|<span data-ttu-id="68648-117">String</span><span class="sxs-lookup"><span data-stu-id="68648-117">String</span></span>|<span data-ttu-id="68648-118">IP 地址上限</span><span class="sxs-lookup"><span data-stu-id="68648-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="68648-119">关系</span><span class="sxs-lookup"><span data-stu-id="68648-119">Relationships</span></span>
<span data-ttu-id="68648-120">无</span><span class="sxs-lookup"><span data-stu-id="68648-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68648-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68648-121">JSON Representation</span></span>
<span data-ttu-id="68648-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68648-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



