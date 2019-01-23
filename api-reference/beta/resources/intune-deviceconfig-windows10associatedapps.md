---
title: windows10AssociatedApps 资源类型
description: Windows 10 相关应用程序定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5dd5b664bde2970caa4b09c027592684b9ecd5e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425916"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="9a5b2-103">windows10AssociatedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a5b2-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="9a5b2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9a5b2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a5b2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a5b2-107">Windows 10 相关应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="9a5b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="9a5b2-108">Properties</span></span>
|<span data-ttu-id="9a5b2-109">属性</span><span class="sxs-lookup"><span data-stu-id="9a5b2-109">Property</span></span>|<span data-ttu-id="9a5b2-110">类型</span><span class="sxs-lookup"><span data-stu-id="9a5b2-110">Type</span></span>|<span data-ttu-id="9a5b2-111">说明</span><span class="sxs-lookup"><span data-stu-id="9a5b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a5b2-112">appType</span><span class="sxs-lookup"><span data-stu-id="9a5b2-112">appType</span></span>|[<span data-ttu-id="9a5b2-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="9a5b2-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="9a5b2-114">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-114">Application type.</span></span> <span data-ttu-id="9a5b2-115">可取值为：`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="9a5b2-116">标识符</span><span class="sxs-lookup"><span data-stu-id="9a5b2-116">identifier</span></span>|<span data-ttu-id="9a5b2-117">String</span><span class="sxs-lookup"><span data-stu-id="9a5b2-117">String</span></span>|<span data-ttu-id="9a5b2-118">标识符。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a5b2-119">关系</span><span class="sxs-lookup"><span data-stu-id="9a5b2-119">Relationships</span></span>
<span data-ttu-id="9a5b2-120">无</span><span class="sxs-lookup"><span data-stu-id="9a5b2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a5b2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a5b2-121">JSON Representation</span></span>
<span data-ttu-id="9a5b2-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a5b2-122">Here is a JSON representation of the resource.</span></span>
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




