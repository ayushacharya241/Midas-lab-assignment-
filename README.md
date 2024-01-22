// Import Maestro's testing functions
import { by, device, expect, element } from 'maestro';

// Write your tests
describe('MyApp Tests', () => {
  beforeEach(async () => {
    await device.reloadReactNative();
  });

  it('should have a welcome screen', async () => {
    await expect(element(by.id('welcome-screen'))).toBeVisible();
  });

  // Add more tests as needed
});
