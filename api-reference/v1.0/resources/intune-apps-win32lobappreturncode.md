---
title: win32LobAppReturnCode 资源类型
description: 包含 Win32 应用的返回代码属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 117ab8bd12cf8113efcbe42aa4f2ab7174e50ac3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759098"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="13100-103">win32LobAppReturnCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="13100-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="13100-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13100-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13100-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13100-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13100-106">包含 Win32 应用的返回代码属性</span><span class="sxs-lookup"><span data-stu-id="13100-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="13100-107">属性</span><span class="sxs-lookup"><span data-stu-id="13100-107">Properties</span></span>
|<span data-ttu-id="13100-108">属性</span><span class="sxs-lookup"><span data-stu-id="13100-108">Property</span></span>|<span data-ttu-id="13100-109">类型</span><span class="sxs-lookup"><span data-stu-id="13100-109">Type</span></span>|<span data-ttu-id="13100-110">说明</span><span class="sxs-lookup"><span data-stu-id="13100-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13100-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="13100-111">returnCode</span></span>|<span data-ttu-id="13100-112">Int32</span><span class="sxs-lookup"><span data-stu-id="13100-112">Int32</span></span>|<span data-ttu-id="13100-113">返回代码。</span><span class="sxs-lookup"><span data-stu-id="13100-113">Return code.</span></span>|
|<span data-ttu-id="13100-114">type</span><span class="sxs-lookup"><span data-stu-id="13100-114">type</span></span>|[<span data-ttu-id="13100-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="13100-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="13100-116">返回代码的类型。</span><span class="sxs-lookup"><span data-stu-id="13100-116">The type of return code.</span></span> <span data-ttu-id="13100-117">可取值为：`failed`、`success`、`softReboot`、`hardReboot`、`retry`。</span><span class="sxs-lookup"><span data-stu-id="13100-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13100-118">关系</span><span class="sxs-lookup"><span data-stu-id="13100-118">Relationships</span></span>
<span data-ttu-id="13100-119">无</span><span class="sxs-lookup"><span data-stu-id="13100-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13100-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13100-120">JSON Representation</span></span>
<span data-ttu-id="13100-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13100-121">Here is a JSON representation of the resource.</span></span>
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




