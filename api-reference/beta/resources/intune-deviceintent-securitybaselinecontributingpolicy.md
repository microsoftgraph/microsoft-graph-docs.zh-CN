---
title: securityBaselineContributingPolicy 资源类型
description: 设备设置的安全基准合规性状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f62299f39d4e3670fc586a4dc07d352a992398e0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209344"
---
# <a name="securitybaselinecontributingpolicy-resource-type"></a><span data-ttu-id="d41fb-103">securityBaselineContributingPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="d41fb-103">securityBaselineContributingPolicy resource type</span></span>

<span data-ttu-id="d41fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d41fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d41fb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d41fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d41fb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d41fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d41fb-107">设备设置的安全基准合规性状态</span><span class="sxs-lookup"><span data-stu-id="d41fb-107">The security baseline compliance state of a setting for a device</span></span>

## <a name="properties"></a><span data-ttu-id="d41fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="d41fb-108">Properties</span></span>
|<span data-ttu-id="d41fb-109">属性</span><span class="sxs-lookup"><span data-stu-id="d41fb-109">Property</span></span>|<span data-ttu-id="d41fb-110">类型</span><span class="sxs-lookup"><span data-stu-id="d41fb-110">Type</span></span>|<span data-ttu-id="d41fb-111">说明</span><span class="sxs-lookup"><span data-stu-id="d41fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d41fb-112">sourceId</span><span class="sxs-lookup"><span data-stu-id="d41fb-112">sourceId</span></span>|<span data-ttu-id="d41fb-113">String</span><span class="sxs-lookup"><span data-stu-id="d41fb-113">String</span></span>|<span data-ttu-id="d41fb-114">策略的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="d41fb-114">Unique identifier of the policy</span></span>|
|<span data-ttu-id="d41fb-115">displayName</span><span class="sxs-lookup"><span data-stu-id="d41fb-115">displayName</span></span>|<span data-ttu-id="d41fb-116">String</span><span class="sxs-lookup"><span data-stu-id="d41fb-116">String</span></span>|<span data-ttu-id="d41fb-117">策略的名称</span><span class="sxs-lookup"><span data-stu-id="d41fb-117">Name of the policy</span></span>|
|<span data-ttu-id="d41fb-118">sourceType</span><span class="sxs-lookup"><span data-stu-id="d41fb-118">sourceType</span></span>|[<span data-ttu-id="d41fb-119">securityBaselinePolicySourceType</span><span class="sxs-lookup"><span data-stu-id="d41fb-119">securityBaselinePolicySourceType</span></span>](../resources/intune-deviceintent-securitybaselinepolicysourcetype.md)|<span data-ttu-id="d41fb-120">策略来源的创作。</span><span class="sxs-lookup"><span data-stu-id="d41fb-120">Authoring source of the policy.</span></span> <span data-ttu-id="d41fb-121">可取值为：`deviceConfiguration`、`deviceIntent`。</span><span class="sxs-lookup"><span data-stu-id="d41fb-121">Possible values are: `deviceConfiguration`, `deviceIntent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d41fb-122">关系</span><span class="sxs-lookup"><span data-stu-id="d41fb-122">Relationships</span></span>
<span data-ttu-id="d41fb-123">无</span><span class="sxs-lookup"><span data-stu-id="d41fb-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d41fb-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d41fb-124">JSON Representation</span></span>
<span data-ttu-id="d41fb-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d41fb-125">Here is a JSON representation of the resource.</span></span>
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




