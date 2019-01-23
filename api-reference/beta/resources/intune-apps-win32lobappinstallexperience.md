---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用程序的安装体验属性
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 240000dfceaa2ef4e973167cbd3b5a743d346892
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406687"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="f7e72-103">win32LobAppInstallExperience 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7e72-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="f7e72-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f7e72-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f7e72-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f7e72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7e72-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7e72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7e72-107">包含 Win32 应用程序的安装体验属性</span><span class="sxs-lookup"><span data-stu-id="f7e72-107">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="f7e72-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7e72-108">Properties</span></span>
|<span data-ttu-id="f7e72-109">属性</span><span class="sxs-lookup"><span data-stu-id="f7e72-109">Property</span></span>|<span data-ttu-id="f7e72-110">类型</span><span class="sxs-lookup"><span data-stu-id="f7e72-110">Type</span></span>|<span data-ttu-id="f7e72-111">说明</span><span class="sxs-lookup"><span data-stu-id="f7e72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7e72-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="f7e72-112">runAsAccount</span></span>|[<span data-ttu-id="f7e72-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="f7e72-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="f7e72-114">指示执行上下文中运行的应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="f7e72-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="f7e72-115">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="f7e72-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7e72-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="f7e72-116">Relationships</span></span>
<span data-ttu-id="f7e72-117">无</span><span class="sxs-lookup"><span data-stu-id="f7e72-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7e72-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7e72-118">JSON Representation</span></span>
<span data-ttu-id="f7e72-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7e72-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```




