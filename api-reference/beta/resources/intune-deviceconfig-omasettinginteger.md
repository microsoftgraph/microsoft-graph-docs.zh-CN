---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 829f73ec2d5eb205e6cacdb46ee209760334cb3a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788441"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="c3060-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3060-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="c3060-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3060-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3060-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3060-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3060-106">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="c3060-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="c3060-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c3060-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3060-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3060-108">Properties</span></span>
|<span data-ttu-id="c3060-109">属性</span><span class="sxs-lookup"><span data-stu-id="c3060-109">Property</span></span>|<span data-ttu-id="c3060-110">类型</span><span class="sxs-lookup"><span data-stu-id="c3060-110">Type</span></span>|<span data-ttu-id="c3060-111">说明</span><span class="sxs-lookup"><span data-stu-id="c3060-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3060-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c3060-112">displayName</span></span>|<span data-ttu-id="c3060-113">字符串</span><span class="sxs-lookup"><span data-stu-id="c3060-113">String</span></span>|<span data-ttu-id="c3060-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="c3060-114">Display Name.</span></span> <span data-ttu-id="c3060-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c3060-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c3060-116">说明</span><span class="sxs-lookup"><span data-stu-id="c3060-116">description</span></span>|<span data-ttu-id="c3060-117">String</span><span class="sxs-lookup"><span data-stu-id="c3060-117">String</span></span>|<span data-ttu-id="c3060-118">说明。</span><span class="sxs-lookup"><span data-stu-id="c3060-118">Description.</span></span> <span data-ttu-id="c3060-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c3060-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c3060-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="c3060-120">omaUri</span></span>|<span data-ttu-id="c3060-121">String</span><span class="sxs-lookup"><span data-stu-id="c3060-121">String</span></span>|<span data-ttu-id="c3060-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="c3060-122">OMA.</span></span> <span data-ttu-id="c3060-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c3060-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c3060-124">值</span><span class="sxs-lookup"><span data-stu-id="c3060-124">value</span></span>|<span data-ttu-id="c3060-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c3060-125">Int32</span></span>|<span data-ttu-id="c3060-126">值。</span><span class="sxs-lookup"><span data-stu-id="c3060-126">Value.</span></span>|
|<span data-ttu-id="c3060-127">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="c3060-127">isReadOnly</span></span>|<span data-ttu-id="c3060-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3060-128">Boolean</span></span>|<span data-ttu-id="c3060-129">通过将设置为 true，则在 OMA-URI 中指定的 CSP （配置服务提供程序）将执行 get，而不是设置</span><span class="sxs-lookup"><span data-stu-id="c3060-129">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3060-130">关系</span><span class="sxs-lookup"><span data-stu-id="c3060-130">Relationships</span></span>
<span data-ttu-id="c3060-131">无</span><span class="sxs-lookup"><span data-stu-id="c3060-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3060-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3060-132">JSON Representation</span></span>
<span data-ttu-id="c3060-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3060-133">Here is a JSON representation of the resource.</span></span>
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
  "value": 1024,
  "isReadOnly": true
}
```



