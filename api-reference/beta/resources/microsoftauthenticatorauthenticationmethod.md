---
title: microsoftAuthenticatorAuthenticationMethod 资源类型
description: 注册到Microsoft Authenticator应用的表示形式。 Microsoft Authenticator身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 07b5c2d776eb7867ffd3b0c847ead72e85bb6229
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298747"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a><span data-ttu-id="6a538-104">microsoftAuthenticatorAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a538-104">microsoftAuthenticatorAuthenticationMethod resource type</span></span>

<span data-ttu-id="6a538-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a538-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a538-106">注册到Microsoft Authenticator应用的表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a538-106">A representation of the Microsoft Authenticator app registered to a user.</span></span> <span data-ttu-id="6a538-107">Microsoft Authenticator身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6a538-107">Microsoft Authenticator is an authentication method.</span></span>

<span data-ttu-id="6a538-108">继承自 [authenticationMethod](../resources/authenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="6a538-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6a538-109">方法</span><span class="sxs-lookup"><span data-stu-id="6a538-109">Methods</span></span>
|<span data-ttu-id="6a538-110">方法</span><span class="sxs-lookup"><span data-stu-id="6a538-110">Method</span></span>|<span data-ttu-id="6a538-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a538-111">Return type</span></span>|<span data-ttu-id="6a538-112">说明</span><span class="sxs-lookup"><span data-stu-id="6a538-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a538-113">列出 microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="6a538-113">List microsoftAuthenticatorAuthenticationMethods</span></span>](../api/microsoftauthenticatorauthenticationmethod-list.md)|<span data-ttu-id="6a538-114">[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a538-114">[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="6a538-115">获取 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="6a538-115">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="6a538-116">获取 microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6a538-116">Get microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-get.md)|[<span data-ttu-id="6a538-117">microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6a538-117">microsoftAuthenticatorAuthenticationMethod</span></span>](../resources/microsoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="6a538-118">读取 [microsoftAuthenticatorAuthenticationMethod 对象的属性和](../resources/microsoftauthenticatorauthenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="6a538-118">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="6a538-119">删除 microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6a538-119">Delete microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-delete.md)|<span data-ttu-id="6a538-120">无</span><span class="sxs-lookup"><span data-stu-id="6a538-120">None</span></span>|<span data-ttu-id="6a538-121">删除 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a538-121">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a538-122">属性</span><span class="sxs-lookup"><span data-stu-id="6a538-122">Properties</span></span>
|<span data-ttu-id="6a538-123">属性</span><span class="sxs-lookup"><span data-stu-id="6a538-123">Property</span></span>|<span data-ttu-id="6a538-124">类型</span><span class="sxs-lookup"><span data-stu-id="6a538-124">Type</span></span>|<span data-ttu-id="6a538-125">说明</span><span class="sxs-lookup"><span data-stu-id="6a538-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a538-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a538-126">createdDateTime</span></span>|<span data-ttu-id="6a538-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a538-127">DateTimeOffset</span></span>|<span data-ttu-id="6a538-128">注册此应用程序的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6a538-128">The date and time that this app was registered.</span></span> <span data-ttu-id="6a538-129">如果设备未注册无密码登录，则电话为空。</span><span class="sxs-lookup"><span data-stu-id="6a538-129">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|
|<span data-ttu-id="6a538-130">displayName</span><span class="sxs-lookup"><span data-stu-id="6a538-130">displayName</span></span>|<span data-ttu-id="6a538-131">String</span><span class="sxs-lookup"><span data-stu-id="6a538-131">String</span></span>|<span data-ttu-id="6a538-132">注册此应用的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="6a538-132">The name of the device on which this app is registered.</span></span>|
|<span data-ttu-id="6a538-133">id</span><span class="sxs-lookup"><span data-stu-id="6a538-133">id</span></span>|<span data-ttu-id="6a538-134">String</span><span class="sxs-lookup"><span data-stu-id="6a538-134">String</span></span>|<span data-ttu-id="6a538-135">此身份验证方法的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6a538-135">A unique identifier for this authentication method.</span></span> <span data-ttu-id="6a538-136">继承自 [authenticationMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="6a538-136">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="6a538-137">deviceTag</span><span class="sxs-lookup"><span data-stu-id="6a538-137">deviceTag</span></span>|<span data-ttu-id="6a538-138">String</span><span class="sxs-lookup"><span data-stu-id="6a538-138">String</span></span>|<span data-ttu-id="6a538-139">包含应用元数据的标记。</span><span class="sxs-lookup"><span data-stu-id="6a538-139">Tags containing app metadata.</span></span>|
|<span data-ttu-id="6a538-140">phoneAppVersion</span><span class="sxs-lookup"><span data-stu-id="6a538-140">phoneAppVersion</span></span>|<span data-ttu-id="6a538-141">String</span><span class="sxs-lookup"><span data-stu-id="6a538-141">String</span></span>|<span data-ttu-id="6a538-142">此应用程序实例的数字Authenticator版本。</span><span class="sxs-lookup"><span data-stu-id="6a538-142">Numerical version of this instance of the Authenticator app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a538-143">关系</span><span class="sxs-lookup"><span data-stu-id="6a538-143">Relationships</span></span>
|<span data-ttu-id="6a538-144">关系</span><span class="sxs-lookup"><span data-stu-id="6a538-144">Relationship</span></span>|<span data-ttu-id="6a538-145">类型</span><span class="sxs-lookup"><span data-stu-id="6a538-145">Type</span></span>|<span data-ttu-id="6a538-146">说明</span><span class="sxs-lookup"><span data-stu-id="6a538-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a538-147">设备</span><span class="sxs-lookup"><span data-stu-id="6a538-147">device</span></span>|[<span data-ttu-id="6a538-148">设备</span><span class="sxs-lookup"><span data-stu-id="6a538-148">device</span></span>](../resources/device.md)|<span data-ttu-id="6a538-149">注册设备所在的Microsoft Authenticator。</span><span class="sxs-lookup"><span data-stu-id="6a538-149">The registered device on which Microsoft Authenticator resides.</span></span> <span data-ttu-id="6a538-150">如果设备未注册无密码登录，则电话为空。</span><span class="sxs-lookup"><span data-stu-id="6a538-150">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a538-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a538-151">JSON representation</span></span>
<span data-ttu-id="6a538-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a538-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "deviceTag": "String",
  "phoneAppVersion": "String",
  "createdDateTime": "DateTimeOffset"
}
```
