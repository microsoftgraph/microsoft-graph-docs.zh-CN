---
title: omaSettingStringXml 资源类型
description: OMA 设置字符串 XML 定义。
author: tfitzmac
ms.openlocfilehash: c7f7d07a94550d86e6507e9202195d09e9555f60
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332009"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="bd128-103">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd128-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="bd128-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bd128-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd128-105">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="bd128-105">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="bd128-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bd128-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd128-107">属性</span><span class="sxs-lookup"><span data-stu-id="bd128-107">Properties</span></span>
|<span data-ttu-id="bd128-108">属性</span><span class="sxs-lookup"><span data-stu-id="bd128-108">Property</span></span>|<span data-ttu-id="bd128-109">类型</span><span class="sxs-lookup"><span data-stu-id="bd128-109">Type</span></span>|<span data-ttu-id="bd128-110">说明</span><span class="sxs-lookup"><span data-stu-id="bd128-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd128-111">displayName</span><span class="sxs-lookup"><span data-stu-id="bd128-111">displayName</span></span>|<span data-ttu-id="bd128-112">String</span><span class="sxs-lookup"><span data-stu-id="bd128-112">String</span></span>|<span data-ttu-id="bd128-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="bd128-113">Display Name.</span></span> <span data-ttu-id="bd128-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bd128-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bd128-115">description</span><span class="sxs-lookup"><span data-stu-id="bd128-115">description</span></span>|<span data-ttu-id="bd128-116">String</span><span class="sxs-lookup"><span data-stu-id="bd128-116">String</span></span>|<span data-ttu-id="bd128-117">说明。</span><span class="sxs-lookup"><span data-stu-id="bd128-117">Description.</span></span> <span data-ttu-id="bd128-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bd128-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bd128-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="bd128-119">omaUri</span></span>|<span data-ttu-id="bd128-120">String</span><span class="sxs-lookup"><span data-stu-id="bd128-120">String</span></span>|<span data-ttu-id="bd128-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="bd128-121">OMA.</span></span> <span data-ttu-id="bd128-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bd128-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bd128-123">fileName</span><span class="sxs-lookup"><span data-stu-id="bd128-123">fileName</span></span>|<span data-ttu-id="bd128-124">String</span><span class="sxs-lookup"><span data-stu-id="bd128-124">String</span></span>|<span data-ttu-id="bd128-125">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="bd128-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="bd128-126">value</span><span class="sxs-lookup"><span data-stu-id="bd128-126">value</span></span>|<span data-ttu-id="bd128-127">Binary</span><span class="sxs-lookup"><span data-stu-id="bd128-127">Binary</span></span>|<span data-ttu-id="bd128-128">值。</span><span class="sxs-lookup"><span data-stu-id="bd128-128">Value.</span></span> <span data-ttu-id="bd128-129">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="bd128-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd128-130">关系</span><span class="sxs-lookup"><span data-stu-id="bd128-130">Relationships</span></span>
<span data-ttu-id="bd128-131">无</span><span class="sxs-lookup"><span data-stu-id="bd128-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd128-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd128-132">JSON Representation</span></span>
<span data-ttu-id="bd128-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd128-133">Here is a JSON representation of the resource.</span></span>
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



