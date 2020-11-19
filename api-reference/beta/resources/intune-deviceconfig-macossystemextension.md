---
title: macOSSystemExtension 资源类型
description: 表示特定的 macOS 系统扩展。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8cea7fb3cb7c0c95fb0ad5174b171bc1993aa1fb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294023"
---
# <a name="macossystemextension-resource-type"></a><span data-ttu-id="e2d83-103">macOSSystemExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2d83-103">macOSSystemExtension resource type</span></span>

<span data-ttu-id="e2d83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2d83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2d83-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2d83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2d83-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2d83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2d83-107">表示特定的 macOS 系统扩展。</span><span class="sxs-lookup"><span data-stu-id="e2d83-107">Represents a specific macOS system extension.</span></span>

## <a name="properties"></a><span data-ttu-id="e2d83-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2d83-108">Properties</span></span>
|<span data-ttu-id="e2d83-109">属性</span><span class="sxs-lookup"><span data-stu-id="e2d83-109">Property</span></span>|<span data-ttu-id="e2d83-110">类型</span><span class="sxs-lookup"><span data-stu-id="e2d83-110">Type</span></span>|<span data-ttu-id="e2d83-111">Description</span><span class="sxs-lookup"><span data-stu-id="e2d83-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2d83-112">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="e2d83-112">teamIdentifier</span></span>|<span data-ttu-id="e2d83-113">字符串</span><span class="sxs-lookup"><span data-stu-id="e2d83-113">String</span></span>|<span data-ttu-id="e2d83-114">获取或设置用于对系统扩展进行签名的团队标识符。</span><span class="sxs-lookup"><span data-stu-id="e2d83-114">Gets or sets the team identifier that was used to sign the system extension.</span></span>|
|<span data-ttu-id="e2d83-115">bundleId</span><span class="sxs-lookup"><span data-stu-id="e2d83-115">bundleId</span></span>|<span data-ttu-id="e2d83-116">String</span><span class="sxs-lookup"><span data-stu-id="e2d83-116">String</span></span>|<span data-ttu-id="e2d83-117">获取或设置系统扩展的捆绑包标识符。</span><span class="sxs-lookup"><span data-stu-id="e2d83-117">Gets or sets the bundle identifier of the system extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2d83-118">关系</span><span class="sxs-lookup"><span data-stu-id="e2d83-118">Relationships</span></span>
<span data-ttu-id="e2d83-119">无</span><span class="sxs-lookup"><span data-stu-id="e2d83-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2d83-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2d83-120">JSON Representation</span></span>
<span data-ttu-id="e2d83-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2d83-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```




