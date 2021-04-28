---
title: azureADDeviceRegistrationError 资源类型
description: Azure AD 设备的注册过程中出现一个错误，该错误阻止该服务在更新管理中注册设备或将内容部署到设备。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d08ab96d5298c70f34acf89e3c6c4605d9df0a1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067862"
---
# <a name="azureaddeviceregistrationerror-resource-type"></a><span data-ttu-id="65b36-103">azureADDeviceRegistrationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="65b36-103">azureADDeviceRegistrationError resource type</span></span>

<span data-ttu-id="65b36-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="65b36-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65b36-105">Azure [AD](../resources/windowsupdates-azureaddevice.md) 设备的注册过程中出现一个错误，该错误阻止该服务在更新管理中注册设备或将内容部署到设备。</span><span class="sxs-lookup"><span data-stu-id="65b36-105">An error in the registration process of an [Azure AD device](../resources/windowsupdates-azureaddevice.md) that prevents the service from enrolling the device in update management or deploying content to the device.</span></span>

<span data-ttu-id="65b36-106">继承自 [updatableAssetError](../resources/windowsupdates-updatableasseterror.md)。</span><span class="sxs-lookup"><span data-stu-id="65b36-106">Inherits from [updatableAssetError](../resources/windowsupdates-updatableasseterror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="65b36-107">属性</span><span class="sxs-lookup"><span data-stu-id="65b36-107">Properties</span></span>
|<span data-ttu-id="65b36-108">属性</span><span class="sxs-lookup"><span data-stu-id="65b36-108">Property</span></span>|<span data-ttu-id="65b36-109">类型</span><span class="sxs-lookup"><span data-stu-id="65b36-109">Type</span></span>|<span data-ttu-id="65b36-110">说明</span><span class="sxs-lookup"><span data-stu-id="65b36-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65b36-111">reason</span><span class="sxs-lookup"><span data-stu-id="65b36-111">reason</span></span>|<span data-ttu-id="65b36-112">microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason</span><span class="sxs-lookup"><span data-stu-id="65b36-112">microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason</span></span>|<span data-ttu-id="65b36-113">注册遇到错误的原因。</span><span class="sxs-lookup"><span data-stu-id="65b36-113">The reason why the registration encountered an error.</span></span> <span data-ttu-id="65b36-114">可取值为：`invalidGlobalDeviceId`、`invalidAzureADDeviceId`、`missingTrustType`、`invalidAzureADJoin`。</span><span class="sxs-lookup"><span data-stu-id="65b36-114">Possible values are: `invalidGlobalDeviceId`, `invalidAzureADDeviceId`, `missingTrustType`, `invalidAzureADJoin`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65b36-115">关系</span><span class="sxs-lookup"><span data-stu-id="65b36-115">Relationships</span></span>
<span data-ttu-id="65b36-116">无。</span><span class="sxs-lookup"><span data-stu-id="65b36-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="65b36-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65b36-117">JSON representation</span></span>
<span data-ttu-id="65b36-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65b36-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDeviceRegistrationError",
  "reason": "String"
}
```

