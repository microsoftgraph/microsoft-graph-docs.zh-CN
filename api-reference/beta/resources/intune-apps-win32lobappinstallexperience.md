---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用程序的安装体验属性
author: tfitzmac
ms.openlocfilehash: c24ed0536416bd330fc2928a85cb0d5fce558256
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342159"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="f61a9-103">win32LobAppInstallExperience 资源类型</span><span class="sxs-lookup"><span data-stu-id="f61a9-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="f61a9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f61a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f61a9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f61a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f61a9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f61a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f61a9-107">包含 Win32 应用程序的安装体验属性</span><span class="sxs-lookup"><span data-stu-id="f61a9-107">Contains installation experience properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="f61a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="f61a9-108">Properties</span></span>
|<span data-ttu-id="f61a9-109">属性</span><span class="sxs-lookup"><span data-stu-id="f61a9-109">Property</span></span>|<span data-ttu-id="f61a9-110">类型</span><span class="sxs-lookup"><span data-stu-id="f61a9-110">Type</span></span>|<span data-ttu-id="f61a9-111">说明</span><span class="sxs-lookup"><span data-stu-id="f61a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f61a9-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="f61a9-112">runAsAccount</span></span>|[<span data-ttu-id="f61a9-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="f61a9-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="f61a9-114">指示执行上下文中运行的应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="f61a9-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="f61a9-115">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="f61a9-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f61a9-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="f61a9-116">Relationships</span></span>
<span data-ttu-id="f61a9-117">无</span><span class="sxs-lookup"><span data-stu-id="f61a9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f61a9-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f61a9-118">JSON Representation</span></span>
<span data-ttu-id="f61a9-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f61a9-119">Here is a JSON representation of the resource.</span></span>
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





