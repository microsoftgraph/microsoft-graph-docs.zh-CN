---
title: deviceManagementTroubleshootingErrorDetails 资源类型
description: 包含有关错误及其修正的详细信息的对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a50c749e6c6c6ddd59705bbea34f0bbd2488f9a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939782"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="219a8-103">deviceManagementTroubleshootingErrorDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="219a8-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="219a8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="219a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="219a8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="219a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="219a8-106">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="219a8-106">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="219a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="219a8-107">Properties</span></span>
|<span data-ttu-id="219a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="219a8-108">Property</span></span>|<span data-ttu-id="219a8-109">类型</span><span class="sxs-lookup"><span data-stu-id="219a8-109">Type</span></span>|<span data-ttu-id="219a8-110">说明</span><span class="sxs-lookup"><span data-stu-id="219a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="219a8-111">context</span><span class="sxs-lookup"><span data-stu-id="219a8-111">context</span></span>|<span data-ttu-id="219a8-112">String</span><span class="sxs-lookup"><span data-stu-id="219a8-112">String</span></span>|<span data-ttu-id="219a8-113">尚未记录</span><span class="sxs-lookup"><span data-stu-id="219a8-113">Not yet documented</span></span>|
|<span data-ttu-id="219a8-114">出</span><span class="sxs-lookup"><span data-stu-id="219a8-114">failure</span></span>|<span data-ttu-id="219a8-115">String</span><span class="sxs-lookup"><span data-stu-id="219a8-115">String</span></span>|<span data-ttu-id="219a8-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="219a8-116">Not yet documented</span></span>|
|<span data-ttu-id="219a8-117">failureDetails</span><span class="sxs-lookup"><span data-stu-id="219a8-117">failureDetails</span></span>|<span data-ttu-id="219a8-118">String</span><span class="sxs-lookup"><span data-stu-id="219a8-118">String</span></span>|<span data-ttu-id="219a8-119">出现问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="219a8-119">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="219a8-120">纠正</span><span class="sxs-lookup"><span data-stu-id="219a8-120">remediation</span></span>|<span data-ttu-id="219a8-121">String</span><span class="sxs-lookup"><span data-stu-id="219a8-121">String</span></span>|<span data-ttu-id="219a8-122">有关如何修正此问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="219a8-122">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="219a8-123">resources</span><span class="sxs-lookup"><span data-stu-id="219a8-123">resources</span></span>|<span data-ttu-id="219a8-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="219a8-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="219a8-125">指向有关此故障的有用文档的链接。</span><span class="sxs-lookup"><span data-stu-id="219a8-125">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="219a8-126">关系</span><span class="sxs-lookup"><span data-stu-id="219a8-126">Relationships</span></span>
<span data-ttu-id="219a8-127">无</span><span class="sxs-lookup"><span data-stu-id="219a8-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="219a8-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="219a8-128">JSON Representation</span></span>
<span data-ttu-id="219a8-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="219a8-129">Here is a JSON representation of the resource.</span></span>
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




