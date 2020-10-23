---
title: securityBaselineContributingPolicy 资源类型
description: 设备设置的安全基准合规性状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0702786afdd049b28fd67638f4fe76920164c35
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704974"
---
# <a name="securitybaselinecontributingpolicy-resource-type"></a><span data-ttu-id="8166f-103">securityBaselineContributingPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="8166f-103">securityBaselineContributingPolicy resource type</span></span>

<span data-ttu-id="8166f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8166f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8166f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8166f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8166f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8166f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8166f-107">设备设置的安全基准合规性状态</span><span class="sxs-lookup"><span data-stu-id="8166f-107">The security baseline compliance state of a setting for a device</span></span>

## <a name="properties"></a><span data-ttu-id="8166f-108">属性</span><span class="sxs-lookup"><span data-stu-id="8166f-108">Properties</span></span>
|<span data-ttu-id="8166f-109">属性</span><span class="sxs-lookup"><span data-stu-id="8166f-109">Property</span></span>|<span data-ttu-id="8166f-110">类型</span><span class="sxs-lookup"><span data-stu-id="8166f-110">Type</span></span>|<span data-ttu-id="8166f-111">说明</span><span class="sxs-lookup"><span data-stu-id="8166f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8166f-112">sourceId</span><span class="sxs-lookup"><span data-stu-id="8166f-112">sourceId</span></span>|<span data-ttu-id="8166f-113">String</span><span class="sxs-lookup"><span data-stu-id="8166f-113">String</span></span>|<span data-ttu-id="8166f-114">策略的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="8166f-114">Unique identifier of the policy</span></span>|
|<span data-ttu-id="8166f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="8166f-115">displayName</span></span>|<span data-ttu-id="8166f-116">String</span><span class="sxs-lookup"><span data-stu-id="8166f-116">String</span></span>|<span data-ttu-id="8166f-117">策略的名称</span><span class="sxs-lookup"><span data-stu-id="8166f-117">Name of the policy</span></span>|
|<span data-ttu-id="8166f-118">sourceType</span><span class="sxs-lookup"><span data-stu-id="8166f-118">sourceType</span></span>|[<span data-ttu-id="8166f-119">securityBaselinePolicySourceType</span><span class="sxs-lookup"><span data-stu-id="8166f-119">securityBaselinePolicySourceType</span></span>](../resources/intune-deviceintent-securitybaselinepolicysourcetype.md)|<span data-ttu-id="8166f-120">策略来源的创作。</span><span class="sxs-lookup"><span data-stu-id="8166f-120">Authoring source of the policy.</span></span> <span data-ttu-id="8166f-121">可取值为：`deviceConfiguration`、`deviceIntent`。</span><span class="sxs-lookup"><span data-stu-id="8166f-121">Possible values are: `deviceConfiguration`, `deviceIntent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8166f-122">关系</span><span class="sxs-lookup"><span data-stu-id="8166f-122">Relationships</span></span>
<span data-ttu-id="8166f-123">无</span><span class="sxs-lookup"><span data-stu-id="8166f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8166f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8166f-124">JSON Representation</span></span>
<span data-ttu-id="8166f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8166f-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.securityBaselineContributingPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineContributingPolicy",
  "sourceId": "String",
  "displayName": "String",
  "sourceType": "String"
}
```





