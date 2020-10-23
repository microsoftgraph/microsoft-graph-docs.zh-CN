---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e5dccc9a0b4329d0f871fa997c627b73ee4bdfc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722955"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="fbc5b-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="fbc5b-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="fbc5b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbc5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbc5b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fbc5b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbc5b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fbc5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbc5b-107">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="fbc5b-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="fbc5b-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fbc5b-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbc5b-109">属性</span><span class="sxs-lookup"><span data-stu-id="fbc5b-109">Properties</span></span>
|<span data-ttu-id="fbc5b-110">属性</span><span class="sxs-lookup"><span data-stu-id="fbc5b-110">Property</span></span>|<span data-ttu-id="fbc5b-111">类型</span><span class="sxs-lookup"><span data-stu-id="fbc5b-111">Type</span></span>|<span data-ttu-id="fbc5b-112">说明</span><span class="sxs-lookup"><span data-stu-id="fbc5b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc5b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="fbc5b-113">displayName</span></span>|<span data-ttu-id="fbc5b-114">String</span><span class="sxs-lookup"><span data-stu-id="fbc5b-114">String</span></span>|<span data-ttu-id="fbc5b-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="fbc5b-115">Display Name.</span></span> <span data-ttu-id="fbc5b-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fbc5b-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fbc5b-117">说明</span><span class="sxs-lookup"><span data-stu-id="fbc5b-117">description</span></span>|<span data-ttu-id="fbc5b-118">String</span><span class="sxs-lookup"><span data-stu-id="fbc5b-118">String</span></span>|<span data-ttu-id="fbc5b-119">说明。</span><span class="sxs-lookup"><span data-stu-id="fbc5b-119">Description.</span></span> <span data-ttu-id="fbc5b-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fbc5b-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fbc5b-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="fbc5b-121">omaUri</span></span>|<span data-ttu-id="fbc5b-122">String</span><span class="sxs-lookup"><span data-stu-id="fbc5b-122">String</span></span>|<span data-ttu-id="fbc5b-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="fbc5b-123">OMA.</span></span> <span data-ttu-id="fbc5b-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fbc5b-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fbc5b-125">值</span><span class="sxs-lookup"><span data-stu-id="fbc5b-125">value</span></span>|<span data-ttu-id="fbc5b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="fbc5b-126">Int32</span></span>|<span data-ttu-id="fbc5b-127">值。</span><span class="sxs-lookup"><span data-stu-id="fbc5b-127">Value.</span></span>|
|<span data-ttu-id="fbc5b-128">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="fbc5b-128">isReadOnly</span></span>|<span data-ttu-id="fbc5b-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbc5b-129">Boolean</span></span>|<span data-ttu-id="fbc5b-130">通过将设置为 true，则在 OMA-URI 中指定的 CSP (配置服务提供程序) 将执行 get，而不是设置</span><span class="sxs-lookup"><span data-stu-id="fbc5b-130">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbc5b-131">关系</span><span class="sxs-lookup"><span data-stu-id="fbc5b-131">Relationships</span></span>
<span data-ttu-id="fbc5b-132">无</span><span class="sxs-lookup"><span data-stu-id="fbc5b-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbc5b-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbc5b-133">JSON Representation</span></span>
<span data-ttu-id="fbc5b-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbc5b-134">Here is a JSON representation of the resource.</span></span>
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





