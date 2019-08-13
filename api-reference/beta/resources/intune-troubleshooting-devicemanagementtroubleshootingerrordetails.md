---
title: deviceManagementTroubleshootingErrorDetails 资源类型
description: 包含有关错误及其修正的详细信息的对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 308947710af3454d7ffbc0e31191ecc1d93c2e25
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347757"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="09cae-103">deviceManagementTroubleshootingErrorDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="09cae-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="09cae-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="09cae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09cae-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09cae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09cae-106">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="09cae-106">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="09cae-107">属性</span><span class="sxs-lookup"><span data-stu-id="09cae-107">Properties</span></span>
|<span data-ttu-id="09cae-108">属性</span><span class="sxs-lookup"><span data-stu-id="09cae-108">Property</span></span>|<span data-ttu-id="09cae-109">类型</span><span class="sxs-lookup"><span data-stu-id="09cae-109">Type</span></span>|<span data-ttu-id="09cae-110">说明</span><span class="sxs-lookup"><span data-stu-id="09cae-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09cae-111">context</span><span class="sxs-lookup"><span data-stu-id="09cae-111">context</span></span>|<span data-ttu-id="09cae-112">String</span><span class="sxs-lookup"><span data-stu-id="09cae-112">String</span></span>|<span data-ttu-id="09cae-113">尚未记录</span><span class="sxs-lookup"><span data-stu-id="09cae-113">Not yet documented</span></span>|
|<span data-ttu-id="09cae-114">出</span><span class="sxs-lookup"><span data-stu-id="09cae-114">failure</span></span>|<span data-ttu-id="09cae-115">String</span><span class="sxs-lookup"><span data-stu-id="09cae-115">String</span></span>|<span data-ttu-id="09cae-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="09cae-116">Not yet documented</span></span>|
|<span data-ttu-id="09cae-117">failureDetails</span><span class="sxs-lookup"><span data-stu-id="09cae-117">failureDetails</span></span>|<span data-ttu-id="09cae-118">String</span><span class="sxs-lookup"><span data-stu-id="09cae-118">String</span></span>|<span data-ttu-id="09cae-119">出现问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="09cae-119">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="09cae-120">纠正</span><span class="sxs-lookup"><span data-stu-id="09cae-120">remediation</span></span>|<span data-ttu-id="09cae-121">String</span><span class="sxs-lookup"><span data-stu-id="09cae-121">String</span></span>|<span data-ttu-id="09cae-122">有关如何修正此问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="09cae-122">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="09cae-123">resources</span><span class="sxs-lookup"><span data-stu-id="09cae-123">resources</span></span>|<span data-ttu-id="09cae-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="09cae-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="09cae-125">指向有关此故障的有用文档的链接。</span><span class="sxs-lookup"><span data-stu-id="09cae-125">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09cae-126">关系</span><span class="sxs-lookup"><span data-stu-id="09cae-126">Relationships</span></span>
<span data-ttu-id="09cae-127">无</span><span class="sxs-lookup"><span data-stu-id="09cae-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09cae-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09cae-128">JSON Representation</span></span>
<span data-ttu-id="09cae-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09cae-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```



