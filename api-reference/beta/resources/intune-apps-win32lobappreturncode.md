---
title: win32LobAppReturnCode 资源类型
description: Win32 应用程序包含返回代码属性
ms.openlocfilehash: 5f32e7e5953ade1036c49ac2fb45555fd353fa1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043291"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="8c9fd-103">win32LobAppReturnCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c9fd-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="8c9fd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8c9fd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c9fd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8c9fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c9fd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8c9fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c9fd-107">Win32 应用程序包含返回代码属性</span><span class="sxs-lookup"><span data-stu-id="8c9fd-107">Contains return code properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="8c9fd-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c9fd-108">Properties</span></span>
|<span data-ttu-id="8c9fd-109">属性</span><span class="sxs-lookup"><span data-stu-id="8c9fd-109">Property</span></span>|<span data-ttu-id="8c9fd-110">类型</span><span class="sxs-lookup"><span data-stu-id="8c9fd-110">Type</span></span>|<span data-ttu-id="8c9fd-111">说明</span><span class="sxs-lookup"><span data-stu-id="8c9fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c9fd-112">returnCode</span><span class="sxs-lookup"><span data-stu-id="8c9fd-112">returnCode</span></span>|<span data-ttu-id="8c9fd-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8c9fd-113">Int32</span></span>|<span data-ttu-id="8c9fd-114">返回代码。</span><span class="sxs-lookup"><span data-stu-id="8c9fd-114">Return code.</span></span>|
|<span data-ttu-id="8c9fd-115">type</span><span class="sxs-lookup"><span data-stu-id="8c9fd-115">type</span></span>|[<span data-ttu-id="8c9fd-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="8c9fd-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="8c9fd-117">返回代码的类型。</span><span class="sxs-lookup"><span data-stu-id="8c9fd-117">The type of return code.</span></span> <span data-ttu-id="8c9fd-118">可取值为：`failed`、`success`、`softReboot`、`hardReboot`、`retry`。</span><span class="sxs-lookup"><span data-stu-id="8c9fd-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c9fd-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="8c9fd-119">Relationships</span></span>
<span data-ttu-id="8c9fd-120">无</span><span class="sxs-lookup"><span data-stu-id="8c9fd-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c9fd-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c9fd-121">JSON Representation</span></span>
<span data-ttu-id="8c9fd-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c9fd-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```





