---
title: windows10AssociatedApps 资源类型
description: 与 Windows 10 相关的应用程序定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d8dc45852b0bd97b7000edd55e74bb9407587d7e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466277"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="847dd-103">windows10AssociatedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="847dd-103">windows10AssociatedApps resource type</span></span>

<span data-ttu-id="847dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="847dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="847dd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="847dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="847dd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="847dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="847dd-107">与 Windows 10 相关的应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="847dd-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="847dd-108">属性</span><span class="sxs-lookup"><span data-stu-id="847dd-108">Properties</span></span>
|<span data-ttu-id="847dd-109">属性</span><span class="sxs-lookup"><span data-stu-id="847dd-109">Property</span></span>|<span data-ttu-id="847dd-110">类型</span><span class="sxs-lookup"><span data-stu-id="847dd-110">Type</span></span>|<span data-ttu-id="847dd-111">说明</span><span class="sxs-lookup"><span data-stu-id="847dd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="847dd-112">appType</span><span class="sxs-lookup"><span data-stu-id="847dd-112">appType</span></span>|[<span data-ttu-id="847dd-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="847dd-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="847dd-114">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="847dd-114">Application type.</span></span> <span data-ttu-id="847dd-115">可取值为：`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="847dd-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="847dd-116">标识符</span><span class="sxs-lookup"><span data-stu-id="847dd-116">identifier</span></span>|<span data-ttu-id="847dd-117">String</span><span class="sxs-lookup"><span data-stu-id="847dd-117">String</span></span>|<span data-ttu-id="847dd-118">标识号.</span><span class="sxs-lookup"><span data-stu-id="847dd-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="847dd-119">关系</span><span class="sxs-lookup"><span data-stu-id="847dd-119">Relationships</span></span>
<span data-ttu-id="847dd-120">无</span><span class="sxs-lookup"><span data-stu-id="847dd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="847dd-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="847dd-121">JSON Representation</span></span>
<span data-ttu-id="847dd-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="847dd-122">Here is a JSON representation of the resource.</span></span>
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



