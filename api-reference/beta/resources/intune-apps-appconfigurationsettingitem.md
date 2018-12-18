---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: tfitzmac
ms.openlocfilehash: 9a9020acc63c445d919564865c44d9c57a5ff57a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320942"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="5d9a4-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d9a4-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="5d9a4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5d9a4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d9a4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5d9a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d9a4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5d9a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d9a4-107">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="5d9a4-107">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="5d9a4-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d9a4-108">Properties</span></span>
|<span data-ttu-id="5d9a4-109">属性</span><span class="sxs-lookup"><span data-stu-id="5d9a4-109">Property</span></span>|<span data-ttu-id="5d9a4-110">类型</span><span class="sxs-lookup"><span data-stu-id="5d9a4-110">Type</span></span>|<span data-ttu-id="5d9a4-111">说明</span><span class="sxs-lookup"><span data-stu-id="5d9a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d9a4-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="5d9a4-112">appConfigKey</span></span>|<span data-ttu-id="5d9a4-113">String</span><span class="sxs-lookup"><span data-stu-id="5d9a4-113">String</span></span>|<span data-ttu-id="5d9a4-114">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="5d9a4-114">app configuration key.</span></span>|
|<span data-ttu-id="5d9a4-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="5d9a4-115">appConfigKeyType</span></span>|[<span data-ttu-id="5d9a4-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="5d9a4-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="5d9a4-117">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="5d9a4-117">app configuration key type.</span></span> <span data-ttu-id="5d9a4-118">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="5d9a4-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="5d9a4-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="5d9a4-119">appConfigKeyValue</span></span>|<span data-ttu-id="5d9a4-120">String</span><span class="sxs-lookup"><span data-stu-id="5d9a4-120">String</span></span>|<span data-ttu-id="5d9a4-121">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="5d9a4-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d9a4-122">关系</span><span class="sxs-lookup"><span data-stu-id="5d9a4-122">Relationships</span></span>
<span data-ttu-id="5d9a4-123">无</span><span class="sxs-lookup"><span data-stu-id="5d9a4-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5d9a4-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d9a4-124">JSON Representation</span></span>
<span data-ttu-id="5d9a4-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d9a4-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```





