---
title: windows10AssociatedApps 资源类型
description: 与 Windows 10 相关的应用程序定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 44b754ba08e8fde1366fda67640582d8552bc4f3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787205"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="8b353-103">windows10AssociatedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b353-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="8b353-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8b353-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b353-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b353-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b353-106">与 Windows 10 相关的应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="8b353-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8b353-107">属性</span><span class="sxs-lookup"><span data-stu-id="8b353-107">Properties</span></span>
|<span data-ttu-id="8b353-108">属性</span><span class="sxs-lookup"><span data-stu-id="8b353-108">Property</span></span>|<span data-ttu-id="8b353-109">类型</span><span class="sxs-lookup"><span data-stu-id="8b353-109">Type</span></span>|<span data-ttu-id="8b353-110">说明</span><span class="sxs-lookup"><span data-stu-id="8b353-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b353-111">appType</span><span class="sxs-lookup"><span data-stu-id="8b353-111">appType</span></span>|[<span data-ttu-id="8b353-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="8b353-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="8b353-113">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="8b353-113">Application type.</span></span> <span data-ttu-id="8b353-114">可取值为：`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="8b353-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="8b353-115">标识符</span><span class="sxs-lookup"><span data-stu-id="8b353-115">identifier</span></span>|<span data-ttu-id="8b353-116">String</span><span class="sxs-lookup"><span data-stu-id="8b353-116">String</span></span>|<span data-ttu-id="8b353-117">标识号.</span><span class="sxs-lookup"><span data-stu-id="8b353-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b353-118">关系</span><span class="sxs-lookup"><span data-stu-id="8b353-118">Relationships</span></span>
<span data-ttu-id="8b353-119">无</span><span class="sxs-lookup"><span data-stu-id="8b353-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b353-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b353-120">JSON Representation</span></span>
<span data-ttu-id="8b353-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b353-121">Here is a JSON representation of the resource.</span></span>
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



