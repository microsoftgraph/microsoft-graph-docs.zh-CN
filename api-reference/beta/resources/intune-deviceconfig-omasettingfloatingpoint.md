---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 506a005994e19e4eabef1a4fda951075f4ce8743
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548010"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="4e181-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e181-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="4e181-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e181-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e181-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e181-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e181-106">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="4e181-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="4e181-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4e181-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e181-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e181-108">Properties</span></span>
|<span data-ttu-id="4e181-109">属性</span><span class="sxs-lookup"><span data-stu-id="4e181-109">Property</span></span>|<span data-ttu-id="4e181-110">类型</span><span class="sxs-lookup"><span data-stu-id="4e181-110">Type</span></span>|<span data-ttu-id="4e181-111">说明</span><span class="sxs-lookup"><span data-stu-id="4e181-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e181-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4e181-112">displayName</span></span>|<span data-ttu-id="4e181-113">字符串</span><span class="sxs-lookup"><span data-stu-id="4e181-113">String</span></span>|<span data-ttu-id="4e181-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="4e181-114">Display Name.</span></span> <span data-ttu-id="4e181-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4e181-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4e181-116">description</span><span class="sxs-lookup"><span data-stu-id="4e181-116">description</span></span>|<span data-ttu-id="4e181-117">String</span><span class="sxs-lookup"><span data-stu-id="4e181-117">String</span></span>|<span data-ttu-id="4e181-118">说明。</span><span class="sxs-lookup"><span data-stu-id="4e181-118">Description.</span></span> <span data-ttu-id="4e181-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4e181-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4e181-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="4e181-120">omaUri</span></span>|<span data-ttu-id="4e181-121">String</span><span class="sxs-lookup"><span data-stu-id="4e181-121">String</span></span>|<span data-ttu-id="4e181-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="4e181-122">OMA.</span></span> <span data-ttu-id="4e181-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4e181-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4e181-124">value</span><span class="sxs-lookup"><span data-stu-id="4e181-124">value</span></span>|<span data-ttu-id="4e181-125">单个</span><span class="sxs-lookup"><span data-stu-id="4e181-125">Single</span></span>|<span data-ttu-id="4e181-126">值。</span><span class="sxs-lookup"><span data-stu-id="4e181-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e181-127">关系</span><span class="sxs-lookup"><span data-stu-id="4e181-127">Relationships</span></span>
<span data-ttu-id="4e181-128">无</span><span class="sxs-lookup"><span data-stu-id="4e181-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e181-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e181-129">JSON Representation</span></span>
<span data-ttu-id="4e181-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e181-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```





