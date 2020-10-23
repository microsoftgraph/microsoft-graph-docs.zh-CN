---
title: deviceCompliancePolicyScript 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e1a87354782ff1e8b4d90eb3c6eb5c69e1332fd4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731410"
---
# <a name="devicecompliancepolicyscript-resource-type"></a><span data-ttu-id="26830-103">deviceCompliancePolicyScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="26830-103">deviceCompliancePolicyScript resource type</span></span>

<span data-ttu-id="26830-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26830-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26830-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26830-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26830-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26830-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26830-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26830-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="26830-108">属性</span><span class="sxs-lookup"><span data-stu-id="26830-108">Properties</span></span>
|<span data-ttu-id="26830-109">属性</span><span class="sxs-lookup"><span data-stu-id="26830-109">Property</span></span>|<span data-ttu-id="26830-110">类型</span><span class="sxs-lookup"><span data-stu-id="26830-110">Type</span></span>|<span data-ttu-id="26830-111">说明</span><span class="sxs-lookup"><span data-stu-id="26830-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26830-112">deviceComplianceScriptId</span><span class="sxs-lookup"><span data-stu-id="26830-112">deviceComplianceScriptId</span></span>|<span data-ttu-id="26830-113">String</span><span class="sxs-lookup"><span data-stu-id="26830-113">String</span></span>|<span data-ttu-id="26830-114">设备合规性脚本 Id。</span><span class="sxs-lookup"><span data-stu-id="26830-114">Device compliance script Id.</span></span>|
|<span data-ttu-id="26830-115">rulesContent</span><span class="sxs-lookup"><span data-stu-id="26830-115">rulesContent</span></span>|<span data-ttu-id="26830-116">Binary</span><span class="sxs-lookup"><span data-stu-id="26830-116">Binary</span></span>|<span data-ttu-id="26830-117">规则的 Json。</span><span class="sxs-lookup"><span data-stu-id="26830-117">Json of the rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26830-118">关系</span><span class="sxs-lookup"><span data-stu-id="26830-118">Relationships</span></span>
<span data-ttu-id="26830-119">无</span><span class="sxs-lookup"><span data-stu-id="26830-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26830-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26830-120">JSON Representation</span></span>
<span data-ttu-id="26830-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26830-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyScript",
  "deviceComplianceScriptId": "String",
  "rulesContent": "binary"
}
```





