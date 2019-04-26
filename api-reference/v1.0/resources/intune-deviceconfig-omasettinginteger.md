---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e4896af0e43510eb791f37a72a864a405388e9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569016"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="c9bd4-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9bd4-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="c9bd4-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9bd4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9bd4-105">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="c9bd4-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="c9bd4-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c9bd4-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9bd4-107">属性</span><span class="sxs-lookup"><span data-stu-id="c9bd4-107">Properties</span></span>
|<span data-ttu-id="c9bd4-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9bd4-108">Property</span></span>|<span data-ttu-id="c9bd4-109">类型</span><span class="sxs-lookup"><span data-stu-id="c9bd4-109">Type</span></span>|<span data-ttu-id="c9bd4-110">说明</span><span class="sxs-lookup"><span data-stu-id="c9bd4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9bd4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c9bd4-111">displayName</span></span>|<span data-ttu-id="c9bd4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="c9bd4-112">String</span></span>|<span data-ttu-id="c9bd4-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="c9bd4-113">Display Name.</span></span> <span data-ttu-id="c9bd4-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c9bd4-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c9bd4-115">说明</span><span class="sxs-lookup"><span data-stu-id="c9bd4-115">description</span></span>|<span data-ttu-id="c9bd4-116">String</span><span class="sxs-lookup"><span data-stu-id="c9bd4-116">String</span></span>|<span data-ttu-id="c9bd4-117">说明。</span><span class="sxs-lookup"><span data-stu-id="c9bd4-117">Description.</span></span> <span data-ttu-id="c9bd4-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c9bd4-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c9bd4-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="c9bd4-119">omaUri</span></span>|<span data-ttu-id="c9bd4-120">String</span><span class="sxs-lookup"><span data-stu-id="c9bd4-120">String</span></span>|<span data-ttu-id="c9bd4-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="c9bd4-121">OMA.</span></span> <span data-ttu-id="c9bd4-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c9bd4-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c9bd4-123">值</span><span class="sxs-lookup"><span data-stu-id="c9bd4-123">value</span></span>|<span data-ttu-id="c9bd4-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c9bd4-124">Int32</span></span>|<span data-ttu-id="c9bd4-125">值。</span><span class="sxs-lookup"><span data-stu-id="c9bd4-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9bd4-126">关系</span><span class="sxs-lookup"><span data-stu-id="c9bd4-126">Relationships</span></span>
<span data-ttu-id="c9bd4-127">无</span><span class="sxs-lookup"><span data-stu-id="c9bd4-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9bd4-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9bd4-128">JSON Representation</span></span>
<span data-ttu-id="c9bd4-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9bd4-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



