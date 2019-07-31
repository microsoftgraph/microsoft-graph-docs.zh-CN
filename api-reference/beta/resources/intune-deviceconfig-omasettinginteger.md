---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58e668baadc854d2f73a3c9f9e52614905fe1a9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011398"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="696b2-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="696b2-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="696b2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="696b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="696b2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="696b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="696b2-106">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="696b2-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="696b2-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="696b2-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="696b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="696b2-108">Properties</span></span>
|<span data-ttu-id="696b2-109">属性</span><span class="sxs-lookup"><span data-stu-id="696b2-109">Property</span></span>|<span data-ttu-id="696b2-110">类型</span><span class="sxs-lookup"><span data-stu-id="696b2-110">Type</span></span>|<span data-ttu-id="696b2-111">说明</span><span class="sxs-lookup"><span data-stu-id="696b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="696b2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="696b2-112">displayName</span></span>|<span data-ttu-id="696b2-113">字符串</span><span class="sxs-lookup"><span data-stu-id="696b2-113">String</span></span>|<span data-ttu-id="696b2-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="696b2-114">Display Name.</span></span> <span data-ttu-id="696b2-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="696b2-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="696b2-116">说明</span><span class="sxs-lookup"><span data-stu-id="696b2-116">description</span></span>|<span data-ttu-id="696b2-117">String</span><span class="sxs-lookup"><span data-stu-id="696b2-117">String</span></span>|<span data-ttu-id="696b2-118">说明。</span><span class="sxs-lookup"><span data-stu-id="696b2-118">Description.</span></span> <span data-ttu-id="696b2-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="696b2-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="696b2-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="696b2-120">omaUri</span></span>|<span data-ttu-id="696b2-121">String</span><span class="sxs-lookup"><span data-stu-id="696b2-121">String</span></span>|<span data-ttu-id="696b2-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="696b2-122">OMA.</span></span> <span data-ttu-id="696b2-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="696b2-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="696b2-124">值</span><span class="sxs-lookup"><span data-stu-id="696b2-124">value</span></span>|<span data-ttu-id="696b2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="696b2-125">Int32</span></span>|<span data-ttu-id="696b2-126">值。</span><span class="sxs-lookup"><span data-stu-id="696b2-126">Value.</span></span>|
|<span data-ttu-id="696b2-127">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="696b2-127">isReadOnly</span></span>|<span data-ttu-id="696b2-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="696b2-128">Boolean</span></span>|<span data-ttu-id="696b2-129">通过将设置为 true, 则在 OMA-URI 中指定的 CSP (配置服务提供程序) 将执行 get, 而不是设置</span><span class="sxs-lookup"><span data-stu-id="696b2-129">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="696b2-130">关系</span><span class="sxs-lookup"><span data-stu-id="696b2-130">Relationships</span></span>
<span data-ttu-id="696b2-131">无</span><span class="sxs-lookup"><span data-stu-id="696b2-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="696b2-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="696b2-132">JSON Representation</span></span>
<span data-ttu-id="696b2-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="696b2-133">Here is a JSON representation of the resource.</span></span>
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





