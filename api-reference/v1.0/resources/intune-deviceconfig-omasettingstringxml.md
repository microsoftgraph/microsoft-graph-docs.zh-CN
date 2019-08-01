---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f6ad3a5e291166813d621e8339adfce6ffe6e2ba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028012"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="6424b-103">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="6424b-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="6424b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6424b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6424b-105">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="6424b-105">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="6424b-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6424b-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6424b-107">属性</span><span class="sxs-lookup"><span data-stu-id="6424b-107">Properties</span></span>
|<span data-ttu-id="6424b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6424b-108">Property</span></span>|<span data-ttu-id="6424b-109">类型</span><span class="sxs-lookup"><span data-stu-id="6424b-109">Type</span></span>|<span data-ttu-id="6424b-110">说明</span><span class="sxs-lookup"><span data-stu-id="6424b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6424b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6424b-111">displayName</span></span>|<span data-ttu-id="6424b-112">字符串</span><span class="sxs-lookup"><span data-stu-id="6424b-112">String</span></span>|<span data-ttu-id="6424b-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="6424b-113">Display Name.</span></span> <span data-ttu-id="6424b-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6424b-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6424b-115">说明</span><span class="sxs-lookup"><span data-stu-id="6424b-115">description</span></span>|<span data-ttu-id="6424b-116">String</span><span class="sxs-lookup"><span data-stu-id="6424b-116">String</span></span>|<span data-ttu-id="6424b-117">说明。</span><span class="sxs-lookup"><span data-stu-id="6424b-117">Description.</span></span> <span data-ttu-id="6424b-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6424b-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6424b-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="6424b-119">omaUri</span></span>|<span data-ttu-id="6424b-120">String</span><span class="sxs-lookup"><span data-stu-id="6424b-120">String</span></span>|<span data-ttu-id="6424b-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="6424b-121">OMA.</span></span> <span data-ttu-id="6424b-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6424b-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6424b-123">fileName</span><span class="sxs-lookup"><span data-stu-id="6424b-123">fileName</span></span>|<span data-ttu-id="6424b-124">String</span><span class="sxs-lookup"><span data-stu-id="6424b-124">String</span></span>|<span data-ttu-id="6424b-125">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="6424b-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="6424b-126">value</span><span class="sxs-lookup"><span data-stu-id="6424b-126">value</span></span>|<span data-ttu-id="6424b-127">Binary</span><span class="sxs-lookup"><span data-stu-id="6424b-127">Binary</span></span>|<span data-ttu-id="6424b-128">值。</span><span class="sxs-lookup"><span data-stu-id="6424b-128">Value.</span></span> <span data-ttu-id="6424b-129">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="6424b-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6424b-130">关系</span><span class="sxs-lookup"><span data-stu-id="6424b-130">Relationships</span></span>
<span data-ttu-id="6424b-131">无</span><span class="sxs-lookup"><span data-stu-id="6424b-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6424b-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6424b-132">JSON Representation</span></span>
<span data-ttu-id="6424b-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6424b-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```



