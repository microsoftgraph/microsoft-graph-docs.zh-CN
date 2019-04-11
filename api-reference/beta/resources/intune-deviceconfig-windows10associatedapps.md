---
title: windows10AssociatedApps 资源类型
description: 与 Windows 10 相关的应用程序定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22adbc6be90718f95a574443c8bd2f96a55f2ee4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784640"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="a5d7e-103">windows10AssociatedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5d7e-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="a5d7e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a5d7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5d7e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5d7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5d7e-106">与 Windows 10 相关的应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="a5d7e-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a5d7e-107">属性</span><span class="sxs-lookup"><span data-stu-id="a5d7e-107">Properties</span></span>
|<span data-ttu-id="a5d7e-108">属性</span><span class="sxs-lookup"><span data-stu-id="a5d7e-108">Property</span></span>|<span data-ttu-id="a5d7e-109">类型</span><span class="sxs-lookup"><span data-stu-id="a5d7e-109">Type</span></span>|<span data-ttu-id="a5d7e-110">说明</span><span class="sxs-lookup"><span data-stu-id="a5d7e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5d7e-111">appType</span><span class="sxs-lookup"><span data-stu-id="a5d7e-111">appType</span></span>|[<span data-ttu-id="a5d7e-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="a5d7e-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="a5d7e-113">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="a5d7e-113">Application type.</span></span> <span data-ttu-id="a5d7e-114">可取值为：`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="a5d7e-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="a5d7e-115">标识符</span><span class="sxs-lookup"><span data-stu-id="a5d7e-115">identifier</span></span>|<span data-ttu-id="a5d7e-116">String</span><span class="sxs-lookup"><span data-stu-id="a5d7e-116">String</span></span>|<span data-ttu-id="a5d7e-117">标识号.</span><span class="sxs-lookup"><span data-stu-id="a5d7e-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5d7e-118">关系</span><span class="sxs-lookup"><span data-stu-id="a5d7e-118">Relationships</span></span>
<span data-ttu-id="a5d7e-119">无</span><span class="sxs-lookup"><span data-stu-id="a5d7e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5d7e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5d7e-120">JSON Representation</span></span>
<span data-ttu-id="a5d7e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5d7e-121">Here is a JSON representation of the resource.</span></span>
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





