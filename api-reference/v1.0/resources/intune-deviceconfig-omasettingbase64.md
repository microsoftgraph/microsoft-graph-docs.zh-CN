---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 678c6e78070a7aae185a041962083b7908ef1cc1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549391"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="e5f93-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5f93-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="e5f93-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5f93-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5f93-105">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="e5f93-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="e5f93-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e5f93-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e5f93-107">属性</span><span class="sxs-lookup"><span data-stu-id="e5f93-107">Properties</span></span>
|<span data-ttu-id="e5f93-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5f93-108">Property</span></span>|<span data-ttu-id="e5f93-109">类型</span><span class="sxs-lookup"><span data-stu-id="e5f93-109">Type</span></span>|<span data-ttu-id="e5f93-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5f93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5f93-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e5f93-111">displayName</span></span>|<span data-ttu-id="e5f93-112">字符串</span><span class="sxs-lookup"><span data-stu-id="e5f93-112">String</span></span>|<span data-ttu-id="e5f93-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="e5f93-113">Display Name.</span></span> <span data-ttu-id="e5f93-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e5f93-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e5f93-115">description</span><span class="sxs-lookup"><span data-stu-id="e5f93-115">description</span></span>|<span data-ttu-id="e5f93-116">String</span><span class="sxs-lookup"><span data-stu-id="e5f93-116">String</span></span>|<span data-ttu-id="e5f93-117">说明。</span><span class="sxs-lookup"><span data-stu-id="e5f93-117">Description.</span></span> <span data-ttu-id="e5f93-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e5f93-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e5f93-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e5f93-119">omaUri</span></span>|<span data-ttu-id="e5f93-120">String</span><span class="sxs-lookup"><span data-stu-id="e5f93-120">String</span></span>|<span data-ttu-id="e5f93-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="e5f93-121">OMA.</span></span> <span data-ttu-id="e5f93-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e5f93-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e5f93-123">fileName</span><span class="sxs-lookup"><span data-stu-id="e5f93-123">fileName</span></span>|<span data-ttu-id="e5f93-124">String</span><span class="sxs-lookup"><span data-stu-id="e5f93-124">String</span></span>|<span data-ttu-id="e5f93-125">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="e5f93-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="e5f93-126">\* .crt</span><span class="sxs-lookup"><span data-stu-id="e5f93-126">\*.crt</span></span> | <span data-ttu-id="e5f93-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="e5f93-127">\*.p7b</span></span> | <span data-ttu-id="e5f93-128">\* bin)。</span><span class="sxs-lookup"><span data-stu-id="e5f93-128">\*.bin).</span></span>|
|<span data-ttu-id="e5f93-129">value</span><span class="sxs-lookup"><span data-stu-id="e5f93-129">value</span></span>|<span data-ttu-id="e5f93-130">String</span><span class="sxs-lookup"><span data-stu-id="e5f93-130">String</span></span>|<span data-ttu-id="e5f93-131">值。</span><span class="sxs-lookup"><span data-stu-id="e5f93-131">Value.</span></span> <span data-ttu-id="e5f93-132">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="e5f93-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5f93-133">关系</span><span class="sxs-lookup"><span data-stu-id="e5f93-133">Relationships</span></span>
<span data-ttu-id="e5f93-134">无</span><span class="sxs-lookup"><span data-stu-id="e5f93-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5f93-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5f93-135">JSON Representation</span></span>
<span data-ttu-id="e5f93-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5f93-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```



