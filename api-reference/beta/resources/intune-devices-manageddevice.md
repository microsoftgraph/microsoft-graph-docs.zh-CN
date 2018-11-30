---
title: managedDevice 资源类型
description: 通过 Intune 托管或预注册的设备
ms.openlocfilehash: eaca9444df77c2f95f6a6f9845c9383cd53cd99f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046856"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="ebe7c-103">managedDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebe7c-103">managedDevice resource type</span></span>

> <span data-ttu-id="ebe7c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebe7c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebe7c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebe7c-107">通过 Intune 托管或预注册的设备</span><span class="sxs-lookup"><span data-stu-id="ebe7c-107">Devices that are managed or pre-enrolled through Intune</span></span>
## <a name="methods"></a><span data-ttu-id="ebe7c-108">方法</span><span class="sxs-lookup"><span data-stu-id="ebe7c-108">Methods</span></span>
|<span data-ttu-id="ebe7c-109">方法</span><span class="sxs-lookup"><span data-stu-id="ebe7c-109">Method</span></span>|<span data-ttu-id="ebe7c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ebe7c-110">Return Type</span></span>|<span data-ttu-id="ebe7c-111">说明</span><span class="sxs-lookup"><span data-stu-id="ebe7c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebe7c-112">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="ebe7c-112">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="ebe7c-113">managedDevice</span><span class="sxs-lookup"><span data-stu-id="ebe7c-113">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="ebe7c-114">读取 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-114">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="ebe7c-115">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="ebe7c-115">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="ebe7c-116">managedDevice</span><span class="sxs-lookup"><span data-stu-id="ebe7c-116">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="ebe7c-117">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-117">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="ebe7c-118">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-118">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="ebe7c-119">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="ebe7c-119">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="ebe7c-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ebe7c-120">Not yet documented</span></span>|
|[<span data-ttu-id="ebe7c-121">enableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-121">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="ebe7c-122">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-122">None</span></span>|<span data-ttu-id="ebe7c-123">启用丢失的模式</span><span class="sxs-lookup"><span data-stu-id="ebe7c-123">Enable lost mode</span></span>|
|[<span data-ttu-id="ebe7c-124">playLostModeSound 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-124">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="ebe7c-125">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-125">None</span></span>|<span data-ttu-id="ebe7c-126">远程锁定</span><span class="sxs-lookup"><span data-stu-id="ebe7c-126">Remote lock</span></span>|
|[<span data-ttu-id="ebe7c-127">setDeviceName 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-127">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="ebe7c-128">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-128">None</span></span>|<span data-ttu-id="ebe7c-129">设置设备的设备名称。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-129">Set device name of the device.</span></span>|
|[<span data-ttu-id="ebe7c-130">retire 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-130">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="ebe7c-131">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-131">None</span></span>|<span data-ttu-id="ebe7c-132">停用设备</span><span class="sxs-lookup"><span data-stu-id="ebe7c-132">Retire a device</span></span>|
|[<span data-ttu-id="ebe7c-133">wipe 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-133">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="ebe7c-134">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-134">None</span></span>|<span data-ttu-id="ebe7c-135">擦除设备</span><span class="sxs-lookup"><span data-stu-id="ebe7c-135">Wipe a device</span></span>|
|[<span data-ttu-id="ebe7c-136">resetPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-136">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="ebe7c-137">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-137">None</span></span>|<span data-ttu-id="ebe7c-138">重置密码</span><span class="sxs-lookup"><span data-stu-id="ebe7c-138">Reset passcode</span></span>|
|[<span data-ttu-id="ebe7c-139">remoteLock 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-139">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="ebe7c-140">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-140">None</span></span>|<span data-ttu-id="ebe7c-141">远程锁定</span><span class="sxs-lookup"><span data-stu-id="ebe7c-141">Remote lock</span></span>|
|[<span data-ttu-id="ebe7c-142">requestRemoteAssistance 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-142">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="ebe7c-143">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-143">None</span></span>|<span data-ttu-id="ebe7c-144">请求远程协助</span><span class="sxs-lookup"><span data-stu-id="ebe7c-144">Request remote assistance</span></span>|
|[<span data-ttu-id="ebe7c-145">disableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-145">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="ebe7c-146">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-146">None</span></span>|<span data-ttu-id="ebe7c-147">禁用丢失模式</span><span class="sxs-lookup"><span data-stu-id="ebe7c-147">Disable lost mode</span></span>|
|[<span data-ttu-id="ebe7c-148">locateDevice 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-148">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="ebe7c-149">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-149">None</span></span>|<span data-ttu-id="ebe7c-150">查找设备</span><span class="sxs-lookup"><span data-stu-id="ebe7c-150">Locate a device</span></span>|
|[<span data-ttu-id="ebe7c-151">bypassActivationLock 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-151">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="ebe7c-152">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-152">None</span></span>|<span data-ttu-id="ebe7c-153">跳过激活锁</span><span class="sxs-lookup"><span data-stu-id="ebe7c-153">Bypass activation lock</span></span>|
|[<span data-ttu-id="ebe7c-154">rebootNow 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-154">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="ebe7c-155">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-155">None</span></span>|<span data-ttu-id="ebe7c-156">重新启动设备</span><span class="sxs-lookup"><span data-stu-id="ebe7c-156">Reboot device</span></span>|
|[<span data-ttu-id="ebe7c-157">shutDown 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-157">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="ebe7c-158">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-158">None</span></span>|<span data-ttu-id="ebe7c-159">关闭设备</span><span class="sxs-lookup"><span data-stu-id="ebe7c-159">Shut down device</span></span>|
|[<span data-ttu-id="ebe7c-160">recoverPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-160">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="ebe7c-161">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-161">None</span></span>|<span data-ttu-id="ebe7c-162">恢复密码</span><span class="sxs-lookup"><span data-stu-id="ebe7c-162">Recover passcode</span></span>|
|[<span data-ttu-id="ebe7c-163">cleanWindowsDevice 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-163">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="ebe7c-164">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-164">None</span></span>|<span data-ttu-id="ebe7c-165">干净的 Windows 设备</span><span class="sxs-lookup"><span data-stu-id="ebe7c-165">Clean Windows device</span></span>|
|[<span data-ttu-id="ebe7c-166">logoutSharedAppleDeviceActiveUser 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-166">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="ebe7c-167">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-167">None</span></span>|<span data-ttu-id="ebe7c-168">注销共享 Apple 设备活动用户</span><span class="sxs-lookup"><span data-stu-id="ebe7c-168">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="ebe7c-169">deleteUserFromSharedAppleDevice 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-169">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="ebe7c-170">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-170">None</span></span>|<span data-ttu-id="ebe7c-171">从共享 Apple 设备中删除用户</span><span class="sxs-lookup"><span data-stu-id="ebe7c-171">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="ebe7c-172">syncDevice 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-172">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="ebe7c-173">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-173">None</span></span>|<span data-ttu-id="ebe7c-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ebe7c-174">Not yet documented</span></span>|
|[<span data-ttu-id="ebe7c-175">windowsDefenderScan 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-175">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="ebe7c-176">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-176">None</span></span>|<span data-ttu-id="ebe7c-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ebe7c-177">Not yet documented</span></span>|
|[<span data-ttu-id="ebe7c-178">windowsDefenderUpdateSignatures 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-178">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="ebe7c-179">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-179">None</span></span>|<span data-ttu-id="ebe7c-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ebe7c-180">Not yet documented</span></span>|
|[<span data-ttu-id="ebe7c-181">updateWindowsDeviceAccount 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-181">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="ebe7c-182">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-182">None</span></span>|<span data-ttu-id="ebe7c-183">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ebe7c-183">Not yet documented</span></span>|
|[<span data-ttu-id="ebe7c-184">revokeAppleVppLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="ebe7c-184">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="ebe7c-185">无</span><span class="sxs-lookup"><span data-stu-id="ebe7c-185">None</span></span>|<span data-ttu-id="ebe7c-186">取消所有设备的 Apple Vpp 许可证</span><span class="sxs-lookup"><span data-stu-id="ebe7c-186">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="ebe7c-187">属性</span><span class="sxs-lookup"><span data-stu-id="ebe7c-187">Properties</span></span>
|<span data-ttu-id="ebe7c-188">属性</span><span class="sxs-lookup"><span data-stu-id="ebe7c-188">Property</span></span>|<span data-ttu-id="ebe7c-189">类型</span><span class="sxs-lookup"><span data-stu-id="ebe7c-189">Type</span></span>|<span data-ttu-id="ebe7c-190">说明</span><span class="sxs-lookup"><span data-stu-id="ebe7c-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebe7c-191">id</span><span class="sxs-lookup"><span data-stu-id="ebe7c-191">id</span></span>|<span data-ttu-id="ebe7c-192">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-192">String</span></span>|<span data-ttu-id="ebe7c-193">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="ebe7c-193">Unique Identifier for the device</span></span>|
|<span data-ttu-id="ebe7c-194">userId</span><span class="sxs-lookup"><span data-stu-id="ebe7c-194">userId</span></span>|<span data-ttu-id="ebe7c-195">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-195">String</span></span>|<span data-ttu-id="ebe7c-196">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="ebe7c-196">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="ebe7c-197">deviceName</span><span class="sxs-lookup"><span data-stu-id="ebe7c-197">deviceName</span></span>|<span data-ttu-id="ebe7c-198">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-198">String</span></span>|<span data-ttu-id="ebe7c-199">设备的名称</span><span class="sxs-lookup"><span data-stu-id="ebe7c-199">Name of the device</span></span>|
|<span data-ttu-id="ebe7c-200">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="ebe7c-200">hardwareInformation</span></span>|[<span data-ttu-id="ebe7c-201">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="ebe7c-201">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="ebe7c-202">设备 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-202">The hardward details for the device.</span></span>  <span data-ttu-id="ebe7c-203">包含信息，如存储空间、 制造商、 序列号等。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-203">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="ebe7c-204">所有者类型</span><span class="sxs-lookup"><span data-stu-id="ebe7c-204">ownerType</span></span>|[<span data-ttu-id="ebe7c-205">所有者类型</span><span class="sxs-lookup"><span data-stu-id="ebe7c-205">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="ebe7c-206">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-206">Ownership of the device.</span></span> <span data-ttu-id="ebe7c-207">可以是公司或个人。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-207">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="ebe7c-208">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-208">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ebe7c-209">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ebe7c-209">managedDeviceOwnerType</span></span>|[<span data-ttu-id="ebe7c-210">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ebe7c-210">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="ebe7c-211">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-211">Ownership of the device.</span></span> <span data-ttu-id="ebe7c-212">可以是公司或个人。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-212">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="ebe7c-213">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-213">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ebe7c-214">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="ebe7c-214">deviceActionResults</span></span>|<span data-ttu-id="ebe7c-215">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebe7c-215">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="ebe7c-216">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-216">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="ebe7c-217">管理</span><span class="sxs-lookup"><span data-stu-id="ebe7c-217">managementState</span></span>|[<span data-ttu-id="ebe7c-218">管理</span><span class="sxs-lookup"><span data-stu-id="ebe7c-218">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="ebe7c-219">管理设备的状态。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-219">Management state of the device.</span></span> <span data-ttu-id="ebe7c-220">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-220">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="ebe7c-221">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="ebe7c-221">enrolledDateTime</span></span>|<span data-ttu-id="ebe7c-222">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebe7c-222">DateTimeOffset</span></span>|<span data-ttu-id="ebe7c-223">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-223">Enrollment time of the device.</span></span>|
|<span data-ttu-id="ebe7c-224">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ebe7c-224">lastSyncDateTime</span></span>|<span data-ttu-id="ebe7c-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebe7c-225">DateTimeOffset</span></span>|<span data-ttu-id="ebe7c-226">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-226">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="ebe7c-227">chassisType</span><span class="sxs-lookup"><span data-stu-id="ebe7c-227">chassisType</span></span>|[<span data-ttu-id="ebe7c-228">chassisType</span><span class="sxs-lookup"><span data-stu-id="ebe7c-228">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="ebe7c-229">机箱设备的类型。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-229">Chassis type of the device.</span></span> <span data-ttu-id="ebe7c-230">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-230">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="ebe7c-231">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="ebe7c-231">operatingSystem</span></span>|<span data-ttu-id="ebe7c-232">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-232">String</span></span>|<span data-ttu-id="ebe7c-233">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-233">Operating system of the device.</span></span> <span data-ttu-id="ebe7c-234">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-234">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="ebe7c-235">deviceType</span><span class="sxs-lookup"><span data-stu-id="ebe7c-235">deviceType</span></span>|[<span data-ttu-id="ebe7c-236">deviceType</span><span class="sxs-lookup"><span data-stu-id="ebe7c-236">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="ebe7c-237">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-237">Platform of the device.</span></span> <span data-ttu-id="ebe7c-238">可能的值为： `desktop`， `windowsRT`， `winMO6`， `nokia`， `windowsPhone`， `mac`， `winCE`， `winEmbedded`， `iPhone`， `iPad`， `iPod`， `android`， `iSocConsumer`， `unix`， `macMDM`， `holoLens`， `surfaceHub`， `androidForWork`， `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ebe7c-238">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="ebe7c-239">complianceState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-239">complianceState</span></span>|[<span data-ttu-id="ebe7c-240">complianceState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-240">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="ebe7c-241">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-241">Compliance state of the device.</span></span> <span data-ttu-id="ebe7c-242">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-242">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="ebe7c-243">jailBroken</span><span class="sxs-lookup"><span data-stu-id="ebe7c-243">jailBroken</span></span>|<span data-ttu-id="ebe7c-244">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-244">String</span></span>|<span data-ttu-id="ebe7c-245">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-245">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="ebe7c-246">managementAgent</span><span class="sxs-lookup"><span data-stu-id="ebe7c-246">managementAgent</span></span>|[<span data-ttu-id="ebe7c-247">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="ebe7c-247">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="ebe7c-248">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-248">Management channel of the device.</span></span> <span data-ttu-id="ebe7c-249">Intune、 EAS 等。可能的值为： `eas`， `mdm`， `easMdm`， `intuneClient`， `easIntuneClient`， `configurationManagerClient`， `configurationManagerClientMdm`， `configurationManagerClientMdmEas`， `unknown`， `jamf`， `googleCloudDevicePolicyController`， `microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-249">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="ebe7c-250">osVersion</span><span class="sxs-lookup"><span data-stu-id="ebe7c-250">osVersion</span></span>|<span data-ttu-id="ebe7c-251">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-251">String</span></span>|<span data-ttu-id="ebe7c-252">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-252">Operating system version of the device.</span></span>|
|<span data-ttu-id="ebe7c-253">easActivated</span><span class="sxs-lookup"><span data-stu-id="ebe7c-253">easActivated</span></span>|<span data-ttu-id="ebe7c-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebe7c-254">Boolean</span></span>|<span data-ttu-id="ebe7c-255">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-255">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="ebe7c-256">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="ebe7c-256">easDeviceId</span></span>|<span data-ttu-id="ebe7c-257">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-257">String</span></span>|<span data-ttu-id="ebe7c-258">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-258">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="ebe7c-259">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="ebe7c-259">easActivationDateTime</span></span>|<span data-ttu-id="ebe7c-260">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebe7c-260">DateTimeOffset</span></span>|<span data-ttu-id="ebe7c-261">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-261">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="ebe7c-262">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="ebe7c-262">aadRegistered</span></span>|<span data-ttu-id="ebe7c-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebe7c-263">Boolean</span></span>|<span data-ttu-id="ebe7c-264">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-264">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="ebe7c-265">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="ebe7c-265">azureADRegistered</span></span>|<span data-ttu-id="ebe7c-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebe7c-266">Boolean</span></span>|<span data-ttu-id="ebe7c-267">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-267">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="ebe7c-268">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ebe7c-268">deviceEnrollmentType</span></span>|[<span data-ttu-id="ebe7c-269">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ebe7c-269">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="ebe7c-270">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-270">Enrollment type of the device.</span></span> <span data-ttu-id="ebe7c-271">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-271">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="ebe7c-272">lostModeState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-272">lostModeState</span></span>|[<span data-ttu-id="ebe7c-273">lostModeState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-273">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="ebe7c-274">指示是否启用或禁用丢失的模式。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-274">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="ebe7c-275">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-275">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="ebe7c-276">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="ebe7c-276">activationLockBypassCode</span></span>|<span data-ttu-id="ebe7c-277">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-277">String</span></span>|<span data-ttu-id="ebe7c-278">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-278">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="ebe7c-279">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ebe7c-279">emailAddress</span></span>|<span data-ttu-id="ebe7c-280">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-280">String</span></span>|<span data-ttu-id="ebe7c-281">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-281">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="ebe7c-282">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="ebe7c-282">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="ebe7c-283">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-283">String</span></span>|<span data-ttu-id="ebe7c-284">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-284">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ebe7c-285">只读。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-285">Read only.</span></span>|
|<span data-ttu-id="ebe7c-286">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="ebe7c-286">azureADDeviceId</span></span>|<span data-ttu-id="ebe7c-287">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-287">String</span></span>|<span data-ttu-id="ebe7c-288">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-288">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ebe7c-289">只读。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-289">Read only.</span></span>|
|<span data-ttu-id="ebe7c-290">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-290">deviceRegistrationState</span></span>|[<span data-ttu-id="ebe7c-291">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-291">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="ebe7c-292">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-292">Device registration state.</span></span> <span data-ttu-id="ebe7c-293">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-293">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="ebe7c-294">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="ebe7c-294">deviceCategoryDisplayName</span></span>|<span data-ttu-id="ebe7c-295">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-295">String</span></span>|<span data-ttu-id="ebe7c-296">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-296">Device category display name</span></span>|
|<span data-ttu-id="ebe7c-297">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ebe7c-297">isSupervised</span></span>|<span data-ttu-id="ebe7c-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebe7c-298">Boolean</span></span>|<span data-ttu-id="ebe7c-299">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="ebe7c-299">Device supervised status</span></span>|
|<span data-ttu-id="ebe7c-300">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ebe7c-300">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ebe7c-301">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebe7c-301">DateTimeOffset</span></span>|<span data-ttu-id="ebe7c-302">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-302">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="ebe7c-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-303">exchangeAccessState</span></span>|[<span data-ttu-id="ebe7c-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="ebe7c-305">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="ebe7c-306">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-306">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="ebe7c-307">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ebe7c-307">exchangeAccessStateReason</span></span>|[<span data-ttu-id="ebe7c-308">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ebe7c-308">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="ebe7c-309">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-309">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="ebe7c-310">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-310">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="ebe7c-311">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="ebe7c-311">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="ebe7c-312">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-312">String</span></span>|<span data-ttu-id="ebe7c-313">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-313">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="ebe7c-314">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ebe7c-314">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="ebe7c-315">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-315">String</span></span>|<span data-ttu-id="ebe7c-316">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-316">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="ebe7c-317">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ebe7c-317">isEncrypted</span></span>|<span data-ttu-id="ebe7c-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebe7c-318">Boolean</span></span>|<span data-ttu-id="ebe7c-319">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="ebe7c-319">Device encryption status</span></span>|
|<span data-ttu-id="ebe7c-320">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ebe7c-320">userPrincipalName</span></span>|<span data-ttu-id="ebe7c-321">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-321">String</span></span>|<span data-ttu-id="ebe7c-322">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="ebe7c-322">Device user principal name</span></span>|
|<span data-ttu-id="ebe7c-323">model</span><span class="sxs-lookup"><span data-stu-id="ebe7c-323">model</span></span>|<span data-ttu-id="ebe7c-324">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-324">String</span></span>|<span data-ttu-id="ebe7c-325">设备的型号</span><span class="sxs-lookup"><span data-stu-id="ebe7c-325">Model of the device</span></span>|
|<span data-ttu-id="ebe7c-326">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ebe7c-326">manufacturer</span></span>|<span data-ttu-id="ebe7c-327">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-327">String</span></span>|<span data-ttu-id="ebe7c-328">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="ebe7c-328">Manufacturer of the device</span></span>|
|<span data-ttu-id="ebe7c-329">imei</span><span class="sxs-lookup"><span data-stu-id="ebe7c-329">imei</span></span>|<span data-ttu-id="ebe7c-330">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-330">String</span></span>|<span data-ttu-id="ebe7c-331">IMEI</span><span class="sxs-lookup"><span data-stu-id="ebe7c-331">IMEI</span></span>|
|<span data-ttu-id="ebe7c-332">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ebe7c-332">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ebe7c-333">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebe7c-333">DateTimeOffset</span></span>|<span data-ttu-id="ebe7c-334">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="ebe7c-334">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ebe7c-335">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ebe7c-335">serialNumber</span></span>|<span data-ttu-id="ebe7c-336">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-336">String</span></span>|<span data-ttu-id="ebe7c-337">序列号</span><span class="sxs-lookup"><span data-stu-id="ebe7c-337">SerialNumber</span></span>|
|<span data-ttu-id="ebe7c-338">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ebe7c-338">phoneNumber</span></span>|<span data-ttu-id="ebe7c-339">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-339">String</span></span>|<span data-ttu-id="ebe7c-340">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="ebe7c-340">Phone number of the device</span></span>|
|<span data-ttu-id="ebe7c-341">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ebe7c-341">androidSecurityPatchLevel</span></span>|<span data-ttu-id="ebe7c-342">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-342">String</span></span>|<span data-ttu-id="ebe7c-343">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="ebe7c-343">Android security patch level</span></span>|
|<span data-ttu-id="ebe7c-344">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ebe7c-344">userDisplayName</span></span>|<span data-ttu-id="ebe7c-345">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-345">String</span></span>|<span data-ttu-id="ebe7c-346">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="ebe7c-346">User display name</span></span>|
|<span data-ttu-id="ebe7c-347">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ebe7c-347">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="ebe7c-348">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ebe7c-348">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="ebe7c-349">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="ebe7c-349">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="ebe7c-350">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="ebe7c-350">wiFiMacAddress</span></span>|<span data-ttu-id="ebe7c-351">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-351">String</span></span>|<span data-ttu-id="ebe7c-352">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="ebe7c-352">Wi-Fi MAC</span></span>|
|<span data-ttu-id="ebe7c-353">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-353">deviceHealthAttestationState</span></span>|[<span data-ttu-id="ebe7c-354">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-354">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="ebe7c-355">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-355">The device health attestation state.</span></span>|
|<span data-ttu-id="ebe7c-356">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="ebe7c-356">subscriberCarrier</span></span>|<span data-ttu-id="ebe7c-357">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-357">String</span></span>|<span data-ttu-id="ebe7c-358">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="ebe7c-358">Subscriber Carrier</span></span>|
|<span data-ttu-id="ebe7c-359">meid</span><span class="sxs-lookup"><span data-stu-id="ebe7c-359">meid</span></span>|<span data-ttu-id="ebe7c-360">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-360">String</span></span>|<span data-ttu-id="ebe7c-361">MEID</span><span class="sxs-lookup"><span data-stu-id="ebe7c-361">MEID</span></span>|
|<span data-ttu-id="ebe7c-362">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ebe7c-362">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="ebe7c-363">Int64</span><span class="sxs-lookup"><span data-stu-id="ebe7c-363">Int64</span></span>|<span data-ttu-id="ebe7c-364">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="ebe7c-364">Total Storage in Bytes</span></span>|
|<span data-ttu-id="ebe7c-365">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ebe7c-365">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="ebe7c-366">Int64</span><span class="sxs-lookup"><span data-stu-id="ebe7c-366">Int64</span></span>|<span data-ttu-id="ebe7c-367">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="ebe7c-367">Free Storage in Bytes</span></span>|
|<span data-ttu-id="ebe7c-368">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="ebe7c-368">managedDeviceName</span></span>|<span data-ttu-id="ebe7c-369">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-369">String</span></span>|<span data-ttu-id="ebe7c-370">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-370">Automatically generated name to identify a device.</span></span> <span data-ttu-id="ebe7c-371">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-371">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="ebe7c-372">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-372">partnerReportedThreatState</span></span>|[<span data-ttu-id="ebe7c-373">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-373">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="ebe7c-374">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-374">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="ebe7c-375">只读。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-375">Read Only.</span></span> <span data-ttu-id="ebe7c-376">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-376">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="ebe7c-377">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="ebe7c-377">usersLoggedOn</span></span>|<span data-ttu-id="ebe7c-378">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="ebe7c-378">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="ebe7c-379">指示上次登录的设备的用户</span><span class="sxs-lookup"><span data-stu-id="ebe7c-379">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="ebe7c-380">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebe7c-380">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="ebe7c-381">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebe7c-381">DateTimeOffset</span></span>|<span data-ttu-id="ebe7c-382">报告 DateTime 的 preferMdmOverGroupPolicy 设置。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-382">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="ebe7c-383">设置时，这些 Intune MDM 设置将覆盖组策略设置冲突时。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-383">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="ebe7c-384">只读。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-384">Read Only.</span></span>|
|<span data-ttu-id="ebe7c-385">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="ebe7c-385">autopilotEnrolled</span></span>|<span data-ttu-id="ebe7c-386">布尔</span><span class="sxs-lookup"><span data-stu-id="ebe7c-386">Boolean</span></span>|<span data-ttu-id="ebe7c-387">如果通过自动试点注册托管的设备，报告。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-387">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="ebe7c-388">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="ebe7c-388">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="ebe7c-389">布尔</span><span class="sxs-lookup"><span data-stu-id="ebe7c-389">Boolean</span></span>|<span data-ttu-id="ebe7c-390">报告托管的 iOS 设备是否用户审批注册。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-390">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="ebe7c-391">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="ebe7c-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="ebe7c-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebe7c-392">DateTimeOffset</span></span>|<span data-ttu-id="ebe7c-393">报告设备管理证书过期日期</span><span class="sxs-lookup"><span data-stu-id="ebe7c-393">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="ebe7c-394">iccid</span><span class="sxs-lookup"><span data-stu-id="ebe7c-394">iccid</span></span>|<span data-ttu-id="ebe7c-395">字符串</span><span class="sxs-lookup"><span data-stu-id="ebe7c-395">String</span></span>|<span data-ttu-id="ebe7c-396">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="ebe7c-397">udid</span><span class="sxs-lookup"><span data-stu-id="ebe7c-397">udid</span></span>|<span data-ttu-id="ebe7c-398">字符串</span><span class="sxs-lookup"><span data-stu-id="ebe7c-398">String</span></span>|<span data-ttu-id="ebe7c-399">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-399">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="ebe7c-400">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ebe7c-400">roleScopeTagIds</span></span>|<span data-ttu-id="ebe7c-401">String 集合</span><span class="sxs-lookup"><span data-stu-id="ebe7c-401">String collection</span></span>|<span data-ttu-id="ebe7c-402">此设备实例范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-402">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="ebe7c-403">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="ebe7c-403">windowsActiveMalwareCount</span></span>|<span data-ttu-id="ebe7c-404">Int32</span><span class="sxs-lookup"><span data-stu-id="ebe7c-404">Int32</span></span>|<span data-ttu-id="ebe7c-405">此 windows 设备的活动恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="ebe7c-405">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="ebe7c-406">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="ebe7c-406">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="ebe7c-407">Int32</span><span class="sxs-lookup"><span data-stu-id="ebe7c-407">Int32</span></span>|<span data-ttu-id="ebe7c-408">此 windows 设备的补救恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="ebe7c-408">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="ebe7c-409">notes</span><span class="sxs-lookup"><span data-stu-id="ebe7c-409">notes</span></span>|<span data-ttu-id="ebe7c-410">String</span><span class="sxs-lookup"><span data-stu-id="ebe7c-410">String</span></span>|<span data-ttu-id="ebe7c-411">由 IT 管理员在设备上的说明</span><span class="sxs-lookup"><span data-stu-id="ebe7c-411">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="ebe7c-412">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-412">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="ebe7c-413">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-413">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="ebe7c-414">配置管理器客户端健康状态，仅供 MDM/ConfigMgr 代理管理设备</span><span class="sxs-lookup"><span data-stu-id="ebe7c-414">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebe7c-415">Relationships</span><span class="sxs-lookup"><span data-stu-id="ebe7c-415">Relationships</span></span>
|<span data-ttu-id="ebe7c-416">关系</span><span class="sxs-lookup"><span data-stu-id="ebe7c-416">Relationship</span></span>|<span data-ttu-id="ebe7c-417">类型</span><span class="sxs-lookup"><span data-stu-id="ebe7c-417">Type</span></span>|<span data-ttu-id="ebe7c-418">说明</span><span class="sxs-lookup"><span data-stu-id="ebe7c-418">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebe7c-419">detectedApps</span><span class="sxs-lookup"><span data-stu-id="ebe7c-419">detectedApps</span></span>|<span data-ttu-id="ebe7c-420">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebe7c-420">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="ebe7c-421">在设备上当前安装的所有应用程序</span><span class="sxs-lookup"><span data-stu-id="ebe7c-421">All applications currently installed on the device</span></span>|
|<span data-ttu-id="ebe7c-422">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ebe7c-422">deviceCategory</span></span>|[<span data-ttu-id="ebe7c-423">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ebe7c-423">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="ebe7c-424">设备类别</span><span class="sxs-lookup"><span data-stu-id="ebe7c-424">Device category</span></span>|
|<span data-ttu-id="ebe7c-425">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-425">windowsProtectionState</span></span>|[<span data-ttu-id="ebe7c-426">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="ebe7c-426">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="ebe7c-427">设备保护状态。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-427">The device protection status.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebe7c-428">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebe7c-428">JSON Representation</span></span>
<span data-ttu-id="ebe7c-429">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebe7c-429">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
  },
  "ownerType": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "String",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024,
    "lastSyncDateTime": "String (timestamp)"
  }
}
```





