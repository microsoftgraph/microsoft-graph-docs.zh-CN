---
title: macOSSystemExtensionTypeMapping 资源类型
description: 表示 macOS 系统扩展和系统扩展类型的团队标识符之间的映射。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3422cdac178ba22dee07aadb4700e2806eedc7ba
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179388"
---
# <a name="macossystemextensiontypemapping-resource-type"></a><span data-ttu-id="09f18-103">macOSSystemExtensionTypeMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="09f18-103">macOSSystemExtensionTypeMapping resource type</span></span>

<span data-ttu-id="09f18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09f18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09f18-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="09f18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09f18-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09f18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09f18-107">表示 macOS 系统扩展和系统扩展类型的团队标识符之间的映射。</span><span class="sxs-lookup"><span data-stu-id="09f18-107">Represents a mapping between team identifiers for macOS system extensions and system extension types.</span></span>

## <a name="properties"></a><span data-ttu-id="09f18-108">属性</span><span class="sxs-lookup"><span data-stu-id="09f18-108">Properties</span></span>
|<span data-ttu-id="09f18-109">属性</span><span class="sxs-lookup"><span data-stu-id="09f18-109">Property</span></span>|<span data-ttu-id="09f18-110">类型</span><span class="sxs-lookup"><span data-stu-id="09f18-110">Type</span></span>|<span data-ttu-id="09f18-111">说明</span><span class="sxs-lookup"><span data-stu-id="09f18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09f18-112">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="09f18-112">teamIdentifier</span></span>|<span data-ttu-id="09f18-113">字符串</span><span class="sxs-lookup"><span data-stu-id="09f18-113">String</span></span>|<span data-ttu-id="09f18-114">获取或设置用于对系统扩展进行签名的团队标识符。</span><span class="sxs-lookup"><span data-stu-id="09f18-114">Gets or sets the team identifier used to sign the system extension.</span></span>|
|<span data-ttu-id="09f18-115">allowedTypes</span><span class="sxs-lookup"><span data-stu-id="09f18-115">allowedTypes</span></span>|[<span data-ttu-id="09f18-116">macOSSystemExtensionType</span><span class="sxs-lookup"><span data-stu-id="09f18-116">macOSSystemExtensionType</span></span>](../resources/intune-deviceconfig-macossystemextensiontype.md)|<span data-ttu-id="09f18-117">获取或设置允许的 macOS 系统扩展类型。</span><span class="sxs-lookup"><span data-stu-id="09f18-117">Gets or sets the allowed macOS system extension types.</span></span> <span data-ttu-id="09f18-118">可取值为：`driverExtensionsAllowed`、`networkExtensionsAllowed`、`endpointSecurityExtensionsAllowed`。</span><span class="sxs-lookup"><span data-stu-id="09f18-118">Possible values are: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09f18-119">关系</span><span class="sxs-lookup"><span data-stu-id="09f18-119">Relationships</span></span>
<span data-ttu-id="09f18-120">无</span><span class="sxs-lookup"><span data-stu-id="09f18-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09f18-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09f18-121">JSON Representation</span></span>
<span data-ttu-id="09f18-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09f18-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtensionTypeMapping",
  "teamIdentifier": "String",
  "allowedTypes": "String"
}
```



