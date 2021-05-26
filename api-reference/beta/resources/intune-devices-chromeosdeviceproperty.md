---
title: chromeOSDeviceProperty 资源类型
description: 表示 ChromeOS 设备的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42b4903965d90641955659277360c46428562ed4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666817"
---
# <a name="chromeosdeviceproperty-resource-type"></a><span data-ttu-id="acc43-103">chromeOSDeviceProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="acc43-103">chromeOSDeviceProperty resource type</span></span>

<span data-ttu-id="acc43-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acc43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="acc43-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="acc43-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acc43-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="acc43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acc43-107">表示 ChromeOS 设备的属性。</span><span class="sxs-lookup"><span data-stu-id="acc43-107">Represents a property of the ChromeOS device.</span></span>

## <a name="properties"></a><span data-ttu-id="acc43-108">属性</span><span class="sxs-lookup"><span data-stu-id="acc43-108">Properties</span></span>
|<span data-ttu-id="acc43-109">属性</span><span class="sxs-lookup"><span data-stu-id="acc43-109">Property</span></span>|<span data-ttu-id="acc43-110">类型</span><span class="sxs-lookup"><span data-stu-id="acc43-110">Type</span></span>|<span data-ttu-id="acc43-111">说明</span><span class="sxs-lookup"><span data-stu-id="acc43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acc43-112">name</span><span class="sxs-lookup"><span data-stu-id="acc43-112">name</span></span>|<span data-ttu-id="acc43-113">String</span><span class="sxs-lookup"><span data-stu-id="acc43-113">String</span></span>|<span data-ttu-id="acc43-114">属性的名称</span><span class="sxs-lookup"><span data-stu-id="acc43-114">Name of the property</span></span>|
|<span data-ttu-id="acc43-115">value</span><span class="sxs-lookup"><span data-stu-id="acc43-115">value</span></span>|<span data-ttu-id="acc43-116">String</span><span class="sxs-lookup"><span data-stu-id="acc43-116">String</span></span>|<span data-ttu-id="acc43-117">属性的值</span><span class="sxs-lookup"><span data-stu-id="acc43-117">Value of the property</span></span>|
|<span data-ttu-id="acc43-118">valueType</span><span class="sxs-lookup"><span data-stu-id="acc43-118">valueType</span></span>|<span data-ttu-id="acc43-119">String</span><span class="sxs-lookup"><span data-stu-id="acc43-119">String</span></span>|<span data-ttu-id="acc43-120">值的类型</span><span class="sxs-lookup"><span data-stu-id="acc43-120">Type of the value</span></span>|
|<span data-ttu-id="acc43-121">updatable</span><span class="sxs-lookup"><span data-stu-id="acc43-121">updatable</span></span>|<span data-ttu-id="acc43-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="acc43-122">Boolean</span></span>|<span data-ttu-id="acc43-123">此属性是否可更新</span><span class="sxs-lookup"><span data-stu-id="acc43-123">Whether this property is updatable</span></span>|

## <a name="relationships"></a><span data-ttu-id="acc43-124">关系</span><span class="sxs-lookup"><span data-stu-id="acc43-124">Relationships</span></span>
<span data-ttu-id="acc43-125">无</span><span class="sxs-lookup"><span data-stu-id="acc43-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="acc43-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acc43-126">JSON Representation</span></span>
<span data-ttu-id="acc43-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acc43-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chromeOSDeviceProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chromeOSDeviceProperty",
  "name": "String",
  "value": "String",
  "valueType": "String",
  "updatable": true
}
```




