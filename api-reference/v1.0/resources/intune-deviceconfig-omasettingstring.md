---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1e0c0fe3f020519770c6770fe515f0349cd6994
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472970"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="6c1cb-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c1cb-103">omaSettingString resource type</span></span>

<span data-ttu-id="6c1cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c1cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c1cb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c1cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c1cb-106">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="6c1cb-106">OMA Settings String definition.</span></span>


<span data-ttu-id="6c1cb-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6c1cb-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6c1cb-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c1cb-108">Properties</span></span>
|<span data-ttu-id="6c1cb-109">属性</span><span class="sxs-lookup"><span data-stu-id="6c1cb-109">Property</span></span>|<span data-ttu-id="6c1cb-110">类型</span><span class="sxs-lookup"><span data-stu-id="6c1cb-110">Type</span></span>|<span data-ttu-id="6c1cb-111">说明</span><span class="sxs-lookup"><span data-stu-id="6c1cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c1cb-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6c1cb-112">displayName</span></span>|<span data-ttu-id="6c1cb-113">字符串</span><span class="sxs-lookup"><span data-stu-id="6c1cb-113">String</span></span>|<span data-ttu-id="6c1cb-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="6c1cb-114">Display Name.</span></span> <span data-ttu-id="6c1cb-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6c1cb-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6c1cb-116">description</span><span class="sxs-lookup"><span data-stu-id="6c1cb-116">description</span></span>|<span data-ttu-id="6c1cb-117">String</span><span class="sxs-lookup"><span data-stu-id="6c1cb-117">String</span></span>|<span data-ttu-id="6c1cb-118">说明。</span><span class="sxs-lookup"><span data-stu-id="6c1cb-118">Description.</span></span> <span data-ttu-id="6c1cb-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6c1cb-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6c1cb-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="6c1cb-120">omaUri</span></span>|<span data-ttu-id="6c1cb-121">String</span><span class="sxs-lookup"><span data-stu-id="6c1cb-121">String</span></span>|<span data-ttu-id="6c1cb-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="6c1cb-122">OMA.</span></span> <span data-ttu-id="6c1cb-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6c1cb-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6c1cb-124">value</span><span class="sxs-lookup"><span data-stu-id="6c1cb-124">value</span></span>|<span data-ttu-id="6c1cb-125">String</span><span class="sxs-lookup"><span data-stu-id="6c1cb-125">String</span></span>|<span data-ttu-id="6c1cb-126">值。</span><span class="sxs-lookup"><span data-stu-id="6c1cb-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c1cb-127">关系</span><span class="sxs-lookup"><span data-stu-id="6c1cb-127">Relationships</span></span>
<span data-ttu-id="6c1cb-128">无</span><span class="sxs-lookup"><span data-stu-id="6c1cb-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c1cb-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c1cb-129">JSON Representation</span></span>
<span data-ttu-id="6c1cb-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c1cb-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```







