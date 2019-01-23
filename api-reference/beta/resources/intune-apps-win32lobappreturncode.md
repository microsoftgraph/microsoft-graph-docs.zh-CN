---
title: win32LobAppReturnCode 资源类型
description: Win32 应用程序包含返回代码属性
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e6357d0ac6aab87e236e02d60454d1b45aa98fe1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404356"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="c0e63-103">win32LobAppReturnCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0e63-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="c0e63-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c0e63-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0e63-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c0e63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0e63-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0e63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0e63-107">Win32 应用程序包含返回代码属性</span><span class="sxs-lookup"><span data-stu-id="c0e63-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="c0e63-108">属性</span><span class="sxs-lookup"><span data-stu-id="c0e63-108">Properties</span></span>
|<span data-ttu-id="c0e63-109">属性</span><span class="sxs-lookup"><span data-stu-id="c0e63-109">Property</span></span>|<span data-ttu-id="c0e63-110">类型</span><span class="sxs-lookup"><span data-stu-id="c0e63-110">Type</span></span>|<span data-ttu-id="c0e63-111">说明</span><span class="sxs-lookup"><span data-stu-id="c0e63-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0e63-112">returnCode</span><span class="sxs-lookup"><span data-stu-id="c0e63-112">returnCode</span></span>|<span data-ttu-id="c0e63-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c0e63-113">Int32</span></span>|<span data-ttu-id="c0e63-114">返回代码。</span><span class="sxs-lookup"><span data-stu-id="c0e63-114">Return code.</span></span>|
|<span data-ttu-id="c0e63-115">type</span><span class="sxs-lookup"><span data-stu-id="c0e63-115">type</span></span>|[<span data-ttu-id="c0e63-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="c0e63-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="c0e63-117">返回代码的类型。</span><span class="sxs-lookup"><span data-stu-id="c0e63-117">The type of return code.</span></span> <span data-ttu-id="c0e63-118">可取值为：`failed`、`success`、`softReboot`、`hardReboot`、`retry`。</span><span class="sxs-lookup"><span data-stu-id="c0e63-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0e63-119">关系</span><span class="sxs-lookup"><span data-stu-id="c0e63-119">Relationships</span></span>
<span data-ttu-id="c0e63-120">无</span><span class="sxs-lookup"><span data-stu-id="c0e63-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0e63-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0e63-121">JSON Representation</span></span>
<span data-ttu-id="c0e63-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0e63-122">Here is a JSON representation of the resource.</span></span>
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




