---
title: androidEnrollmentCompanyCode 资源类型
description: 用于保存用于通过 Google 的 Android 管理 API (如令牌、Url 和 QR 代码内容) 进行注册的专业注册数据的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6110385caa6c1ac2a84f17160acc996a4b922107
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950807"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="d00a8-103">androidEnrollmentCompanyCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="d00a8-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="d00a8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d00a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d00a8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d00a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d00a8-106">用于保存用于通过 Google 的 Android 管理 API (如令牌、Url 和 QR 代码内容) 进行注册的专业注册数据的类</span><span class="sxs-lookup"><span data-stu-id="d00a8-106">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="d00a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="d00a8-107">Properties</span></span>
|<span data-ttu-id="d00a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="d00a8-108">Property</span></span>|<span data-ttu-id="d00a8-109">类型</span><span class="sxs-lookup"><span data-stu-id="d00a8-109">Type</span></span>|<span data-ttu-id="d00a8-110">说明</span><span class="sxs-lookup"><span data-stu-id="d00a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d00a8-111">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="d00a8-111">enrollmentToken</span></span>|<span data-ttu-id="d00a8-112">String</span><span class="sxs-lookup"><span data-stu-id="d00a8-112">String</span></span>|<span data-ttu-id="d00a8-113">用户用于注册其设备的注册令牌。</span><span class="sxs-lookup"><span data-stu-id="d00a8-113">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="d00a8-114">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="d00a8-114">qrCodeContent</span></span>|<span data-ttu-id="d00a8-115">String</span><span class="sxs-lookup"><span data-stu-id="d00a8-115">String</span></span>|<span data-ttu-id="d00a8-116">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="d00a8-116">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="d00a8-117">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="d00a8-117">qrCodeImage</span></span>|[<span data-ttu-id="d00a8-118">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d00a8-118">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d00a8-119">为令牌生成的 QR 代码。</span><span class="sxs-lookup"><span data-stu-id="d00a8-119">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d00a8-120">关系</span><span class="sxs-lookup"><span data-stu-id="d00a8-120">Relationships</span></span>
<span data-ttu-id="d00a8-121">无</span><span class="sxs-lookup"><span data-stu-id="d00a8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d00a8-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d00a8-122">JSON Representation</span></span>
<span data-ttu-id="d00a8-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d00a8-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




