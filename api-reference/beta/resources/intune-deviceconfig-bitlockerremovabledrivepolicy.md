---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
ms.openlocfilehash: 726fb8aa0493ce17984719403a6fcf800300a9ad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048369"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="903ba-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="903ba-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="903ba-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="903ba-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="903ba-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="903ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="903ba-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="903ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="903ba-107">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="903ba-107">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="903ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="903ba-108">Properties</span></span>
|<span data-ttu-id="903ba-109">属性</span><span class="sxs-lookup"><span data-stu-id="903ba-109">Property</span></span>|<span data-ttu-id="903ba-110">类型</span><span class="sxs-lookup"><span data-stu-id="903ba-110">Type</span></span>|<span data-ttu-id="903ba-111">说明</span><span class="sxs-lookup"><span data-stu-id="903ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="903ba-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="903ba-112">encryptionMethod</span></span>|[<span data-ttu-id="903ba-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="903ba-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="903ba-114">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="903ba-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="903ba-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="903ba-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="903ba-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="903ba-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="903ba-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="903ba-117">Boolean</span></span>|<span data-ttu-id="903ba-118">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="903ba-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="903ba-119">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="903ba-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="903ba-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="903ba-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="903ba-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="903ba-121">Boolean</span></span>|<span data-ttu-id="903ba-122">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="903ba-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="903ba-123">关系</span><span class="sxs-lookup"><span data-stu-id="903ba-123">Relationships</span></span>
<span data-ttu-id="903ba-124">无</span><span class="sxs-lookup"><span data-stu-id="903ba-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="903ba-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="903ba-125">JSON Representation</span></span>
<span data-ttu-id="903ba-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="903ba-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```





