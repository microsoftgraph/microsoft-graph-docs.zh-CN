---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c0e47ba7fce929e114282c6aa88605d9f185618
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419434"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="f0370-103">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0370-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="f0370-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f0370-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f0370-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f0370-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0370-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0370-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0370-107">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="f0370-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="f0370-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0370-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0370-109">属性</span><span class="sxs-lookup"><span data-stu-id="f0370-109">Properties</span></span>
|<span data-ttu-id="f0370-110">属性</span><span class="sxs-lookup"><span data-stu-id="f0370-110">Property</span></span>|<span data-ttu-id="f0370-111">类型</span><span class="sxs-lookup"><span data-stu-id="f0370-111">Type</span></span>|<span data-ttu-id="f0370-112">说明</span><span class="sxs-lookup"><span data-stu-id="f0370-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0370-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f0370-113">displayName</span></span>|<span data-ttu-id="f0370-114">String</span><span class="sxs-lookup"><span data-stu-id="f0370-114">String</span></span>|<span data-ttu-id="f0370-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="f0370-115">Display Name.</span></span> <span data-ttu-id="f0370-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0370-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f0370-117">description</span><span class="sxs-lookup"><span data-stu-id="f0370-117">description</span></span>|<span data-ttu-id="f0370-118">String</span><span class="sxs-lookup"><span data-stu-id="f0370-118">String</span></span>|<span data-ttu-id="f0370-119">说明。</span><span class="sxs-lookup"><span data-stu-id="f0370-119">Description.</span></span> <span data-ttu-id="f0370-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0370-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f0370-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="f0370-121">omaUri</span></span>|<span data-ttu-id="f0370-122">String</span><span class="sxs-lookup"><span data-stu-id="f0370-122">String</span></span>|<span data-ttu-id="f0370-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="f0370-123">OMA.</span></span> <span data-ttu-id="f0370-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0370-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f0370-125">fileName</span><span class="sxs-lookup"><span data-stu-id="f0370-125">fileName</span></span>|<span data-ttu-id="f0370-126">String</span><span class="sxs-lookup"><span data-stu-id="f0370-126">String</span></span>|<span data-ttu-id="f0370-127">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="f0370-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="f0370-128">value</span><span class="sxs-lookup"><span data-stu-id="f0370-128">value</span></span>|<span data-ttu-id="f0370-129">Binary</span><span class="sxs-lookup"><span data-stu-id="f0370-129">Binary</span></span>|<span data-ttu-id="f0370-130">值。</span><span class="sxs-lookup"><span data-stu-id="f0370-130">Value.</span></span> <span data-ttu-id="f0370-131">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="f0370-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0370-132">关系</span><span class="sxs-lookup"><span data-stu-id="f0370-132">Relationships</span></span>
<span data-ttu-id="f0370-133">无</span><span class="sxs-lookup"><span data-stu-id="f0370-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0370-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0370-134">JSON Representation</span></span>
<span data-ttu-id="f0370-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0370-135">Here is a JSON representation of the resource.</span></span>
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




