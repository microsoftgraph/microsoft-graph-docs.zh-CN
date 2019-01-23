---
title: deviceManagementTroubleshootingErrorDetails 资源类型
description: 对象包含有关错误和其修复的详细的信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9cdda64170afc739c23f1b258e5f2f1b31158662
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429362"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="8607d-103">deviceManagementTroubleshootingErrorDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="8607d-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="8607d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8607d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8607d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8607d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8607d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8607d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8607d-107">对象包含有关错误和其修复的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="8607d-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="8607d-108">属性</span><span class="sxs-lookup"><span data-stu-id="8607d-108">Properties</span></span>
|<span data-ttu-id="8607d-109">属性</span><span class="sxs-lookup"><span data-stu-id="8607d-109">Property</span></span>|<span data-ttu-id="8607d-110">类型</span><span class="sxs-lookup"><span data-stu-id="8607d-110">Type</span></span>|<span data-ttu-id="8607d-111">说明</span><span class="sxs-lookup"><span data-stu-id="8607d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8607d-112">context</span><span class="sxs-lookup"><span data-stu-id="8607d-112">context</span></span>|<span data-ttu-id="8607d-113">String</span><span class="sxs-lookup"><span data-stu-id="8607d-113">String</span></span>|<span data-ttu-id="8607d-114">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8607d-114">Not yet documented</span></span>|
|<span data-ttu-id="8607d-115">failure</span><span class="sxs-lookup"><span data-stu-id="8607d-115">failure</span></span>|<span data-ttu-id="8607d-116">String</span><span class="sxs-lookup"><span data-stu-id="8607d-116">String</span></span>|<span data-ttu-id="8607d-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8607d-117">Not yet documented</span></span>|
|<span data-ttu-id="8607d-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="8607d-118">failureDetails</span></span>|<span data-ttu-id="8607d-119">String</span><span class="sxs-lookup"><span data-stu-id="8607d-119">String</span></span>|<span data-ttu-id="8607d-120">发生了什么错误详细的描述。</span><span class="sxs-lookup"><span data-stu-id="8607d-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="8607d-121">修正</span><span class="sxs-lookup"><span data-stu-id="8607d-121">remediation</span></span>|<span data-ttu-id="8607d-122">String</span><span class="sxs-lookup"><span data-stu-id="8607d-122">String</span></span>|<span data-ttu-id="8607d-123">如何解决此问题的详细的说明。</span><span class="sxs-lookup"><span data-stu-id="8607d-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="8607d-124">resources</span><span class="sxs-lookup"><span data-stu-id="8607d-124">resources</span></span>|<span data-ttu-id="8607d-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="8607d-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="8607d-126">链接到有关该故障的帮助文档。</span><span class="sxs-lookup"><span data-stu-id="8607d-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8607d-127">关系</span><span class="sxs-lookup"><span data-stu-id="8607d-127">Relationships</span></span>
<span data-ttu-id="8607d-128">无</span><span class="sxs-lookup"><span data-stu-id="8607d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8607d-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8607d-129">JSON Representation</span></span>
<span data-ttu-id="8607d-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8607d-130">Here is a JSON representation of the resource.</span></span>
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




