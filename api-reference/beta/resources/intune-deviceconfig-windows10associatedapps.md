---
title: windows10AssociatedApps 资源类型
description: 与 Windows 10 相关的应用程序定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ba372cd3e8f67371adac9f92da92da4c7efe2a28
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525689"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="71190-103">windows10AssociatedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="71190-103">windows10AssociatedApps resource type</span></span>

<span data-ttu-id="71190-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="71190-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71190-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="71190-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71190-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71190-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71190-107">与 Windows 10 相关的应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="71190-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="71190-108">属性</span><span class="sxs-lookup"><span data-stu-id="71190-108">Properties</span></span>
|<span data-ttu-id="71190-109">属性</span><span class="sxs-lookup"><span data-stu-id="71190-109">Property</span></span>|<span data-ttu-id="71190-110">类型</span><span class="sxs-lookup"><span data-stu-id="71190-110">Type</span></span>|<span data-ttu-id="71190-111">说明</span><span class="sxs-lookup"><span data-stu-id="71190-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71190-112">appType</span><span class="sxs-lookup"><span data-stu-id="71190-112">appType</span></span>|[<span data-ttu-id="71190-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="71190-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="71190-114">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="71190-114">Application type.</span></span> <span data-ttu-id="71190-115">可取值为：`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="71190-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="71190-116">标识符</span><span class="sxs-lookup"><span data-stu-id="71190-116">identifier</span></span>|<span data-ttu-id="71190-117">String</span><span class="sxs-lookup"><span data-stu-id="71190-117">String</span></span>|<span data-ttu-id="71190-118">标识号.</span><span class="sxs-lookup"><span data-stu-id="71190-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71190-119">关系</span><span class="sxs-lookup"><span data-stu-id="71190-119">Relationships</span></span>
<span data-ttu-id="71190-120">无</span><span class="sxs-lookup"><span data-stu-id="71190-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71190-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71190-121">JSON Representation</span></span>
<span data-ttu-id="71190-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71190-122">Here is a JSON representation of the resource.</span></span>
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



