---
title: windows10AssociatedApps 资源类型
description: 与 Windows 10 相关的应用程序定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fca7f8876ba0ea455d2bd7f537fe162f125e1dc9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944382"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="a5f63-103">windows10AssociatedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5f63-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="a5f63-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a5f63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5f63-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5f63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5f63-106">与 Windows 10 相关的应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="a5f63-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a5f63-107">属性</span><span class="sxs-lookup"><span data-stu-id="a5f63-107">Properties</span></span>
|<span data-ttu-id="a5f63-108">属性</span><span class="sxs-lookup"><span data-stu-id="a5f63-108">Property</span></span>|<span data-ttu-id="a5f63-109">类型</span><span class="sxs-lookup"><span data-stu-id="a5f63-109">Type</span></span>|<span data-ttu-id="a5f63-110">说明</span><span class="sxs-lookup"><span data-stu-id="a5f63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5f63-111">appType</span><span class="sxs-lookup"><span data-stu-id="a5f63-111">appType</span></span>|[<span data-ttu-id="a5f63-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="a5f63-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="a5f63-113">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="a5f63-113">Application type.</span></span> <span data-ttu-id="a5f63-114">可取值为：`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="a5f63-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="a5f63-115">标识符</span><span class="sxs-lookup"><span data-stu-id="a5f63-115">identifier</span></span>|<span data-ttu-id="a5f63-116">String</span><span class="sxs-lookup"><span data-stu-id="a5f63-116">String</span></span>|<span data-ttu-id="a5f63-117">标识号.</span><span class="sxs-lookup"><span data-stu-id="a5f63-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5f63-118">关系</span><span class="sxs-lookup"><span data-stu-id="a5f63-118">Relationships</span></span>
<span data-ttu-id="a5f63-119">无</span><span class="sxs-lookup"><span data-stu-id="a5f63-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5f63-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5f63-120">JSON Representation</span></span>
<span data-ttu-id="a5f63-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5f63-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```




