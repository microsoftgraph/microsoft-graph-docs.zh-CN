---
title: deviceManagementTroubleshootingErrorDetails 资源类型
description: 包含有关错误及其修正的详细信息的对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6fea29d21c34ab123ba5c573b2a19858cd3bf756
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523385"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="0a086-103">deviceManagementTroubleshootingErrorDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a086-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

<span data-ttu-id="0a086-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0a086-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a086-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0a086-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a086-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a086-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a086-107">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="0a086-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="0a086-108">属性</span><span class="sxs-lookup"><span data-stu-id="0a086-108">Properties</span></span>
|<span data-ttu-id="0a086-109">属性</span><span class="sxs-lookup"><span data-stu-id="0a086-109">Property</span></span>|<span data-ttu-id="0a086-110">类型</span><span class="sxs-lookup"><span data-stu-id="0a086-110">Type</span></span>|<span data-ttu-id="0a086-111">说明</span><span class="sxs-lookup"><span data-stu-id="0a086-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a086-112">context</span><span class="sxs-lookup"><span data-stu-id="0a086-112">context</span></span>|<span data-ttu-id="0a086-113">String</span><span class="sxs-lookup"><span data-stu-id="0a086-113">String</span></span>|<span data-ttu-id="0a086-114">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0a086-114">Not yet documented</span></span>|
|<span data-ttu-id="0a086-115">出</span><span class="sxs-lookup"><span data-stu-id="0a086-115">failure</span></span>|<span data-ttu-id="0a086-116">String</span><span class="sxs-lookup"><span data-stu-id="0a086-116">String</span></span>|<span data-ttu-id="0a086-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0a086-117">Not yet documented</span></span>|
|<span data-ttu-id="0a086-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="0a086-118">failureDetails</span></span>|<span data-ttu-id="0a086-119">String</span><span class="sxs-lookup"><span data-stu-id="0a086-119">String</span></span>|<span data-ttu-id="0a086-120">出现问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="0a086-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="0a086-121">纠正</span><span class="sxs-lookup"><span data-stu-id="0a086-121">remediation</span></span>|<span data-ttu-id="0a086-122">String</span><span class="sxs-lookup"><span data-stu-id="0a086-122">String</span></span>|<span data-ttu-id="0a086-123">有关如何修正此问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="0a086-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="0a086-124">resources</span><span class="sxs-lookup"><span data-stu-id="0a086-124">resources</span></span>|<span data-ttu-id="0a086-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="0a086-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="0a086-126">指向有关此故障的有用文档的链接。</span><span class="sxs-lookup"><span data-stu-id="0a086-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a086-127">关系</span><span class="sxs-lookup"><span data-stu-id="0a086-127">Relationships</span></span>
<span data-ttu-id="0a086-128">无</span><span class="sxs-lookup"><span data-stu-id="0a086-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a086-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a086-129">JSON Representation</span></span>
<span data-ttu-id="0a086-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a086-130">Here is a JSON representation of the resource.</span></span>
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



