---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3c54bdab0870dfd4f3b28ae0af9036682f0464a4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969945"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="ec561-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec561-103">omaSettingString resource type</span></span>

> <span data-ttu-id="ec561-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec561-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec561-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec561-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec561-106">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="ec561-106">OMA Settings String definition.</span></span>


<span data-ttu-id="ec561-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ec561-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ec561-108">属性</span><span class="sxs-lookup"><span data-stu-id="ec561-108">Properties</span></span>
|<span data-ttu-id="ec561-109">属性</span><span class="sxs-lookup"><span data-stu-id="ec561-109">Property</span></span>|<span data-ttu-id="ec561-110">类型</span><span class="sxs-lookup"><span data-stu-id="ec561-110">Type</span></span>|<span data-ttu-id="ec561-111">说明</span><span class="sxs-lookup"><span data-stu-id="ec561-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec561-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ec561-112">displayName</span></span>|<span data-ttu-id="ec561-113">字符串</span><span class="sxs-lookup"><span data-stu-id="ec561-113">String</span></span>|<span data-ttu-id="ec561-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="ec561-114">Display Name.</span></span> <span data-ttu-id="ec561-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ec561-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ec561-116">说明</span><span class="sxs-lookup"><span data-stu-id="ec561-116">description</span></span>|<span data-ttu-id="ec561-117">String</span><span class="sxs-lookup"><span data-stu-id="ec561-117">String</span></span>|<span data-ttu-id="ec561-118">说明。</span><span class="sxs-lookup"><span data-stu-id="ec561-118">Description.</span></span> <span data-ttu-id="ec561-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ec561-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ec561-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="ec561-120">omaUri</span></span>|<span data-ttu-id="ec561-121">String</span><span class="sxs-lookup"><span data-stu-id="ec561-121">String</span></span>|<span data-ttu-id="ec561-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="ec561-122">OMA.</span></span> <span data-ttu-id="ec561-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ec561-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ec561-124">value</span><span class="sxs-lookup"><span data-stu-id="ec561-124">value</span></span>|<span data-ttu-id="ec561-125">String</span><span class="sxs-lookup"><span data-stu-id="ec561-125">String</span></span>|<span data-ttu-id="ec561-126">值。</span><span class="sxs-lookup"><span data-stu-id="ec561-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec561-127">关系</span><span class="sxs-lookup"><span data-stu-id="ec561-127">Relationships</span></span>
<span data-ttu-id="ec561-128">无</span><span class="sxs-lookup"><span data-stu-id="ec561-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec561-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec561-129">JSON Representation</span></span>
<span data-ttu-id="ec561-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec561-130">Here is a JSON representation of the resource.</span></span>
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





